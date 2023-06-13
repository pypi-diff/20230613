# Comparing `tmp/alibabacloud_ens20171110-3.0.8.tar.gz` & `tmp/alibabacloud_ens20171110-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ens20171110-3.0.8.tar", last modified: Thu Sep 22 03:02:20 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ens20171110-3.0.9.tar", last modified: Thu Oct 13 08:57:26 2022, max compression
```

## Comparing `alibabacloud_ens20171110-3.0.8.tar` & `alibabacloud_ens20171110-3.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/
--rw-r--r--   0 root         (0) root         (0)      670 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2342 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110/__init__.py
--rw-r--r--   0 root         (0) root         (0)   650277 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110/client.py
--rw-r--r--   0 root         (0) root         (0)  1140558 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2342 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2624 2022-09-22 03:02:20.000000 alibabacloud_ens20171110-3.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/
+-rw-r--r--   0 root         (0) root         (0)      721 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2342 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   655763 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110/client.py
+-rw-r--r--   0 root         (0) root         (0)  1156519 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2342 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2624 2022-10-13 08:57:26.000000 alibabacloud_ens20171110-3.0.9/setup.py
```

### Comparing `alibabacloud_ens20171110-3.0.8/LICENSE` & `alibabacloud_ens20171110-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ens20171110-3.0.8/PKG-INFO` & `alibabacloud_ens20171110-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ens20171110
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud edge node service (20171110) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ens20171110-3.0.8/README-CN.md` & `alibabacloud_ens20171110-3.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ens20171110-3.0.8/README.md` & `alibabacloud_ens20171110-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110/client.py` & `alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4551,14 +4551,96 @@
     async def delete_vswitch_async(
         self,
         request: ens_20171110_models.DeleteVSwitchRequest,
     ) -> ens_20171110_models.DeleteVSwitchResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_vswitch_with_options_async(request, runtime)
 
+    def describe_aicimages_with_options(
+        self,
+        request: ens_20171110_models.DescribeAICImagesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ens_20171110_models.DescribeAICImagesResponse:
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
+    async def describe_aicimages_with_options_async(
+        self,
+        request: ens_20171110_models.DescribeAICImagesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ens_20171110_models.DescribeAICImagesResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_aicimages(
+        self,
+        request: ens_20171110_models.DescribeAICImagesRequest,
+    ) -> ens_20171110_models.DescribeAICImagesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_aicimages_with_options(request, runtime)
+
+    async def describe_aicimages_async(
+        self,
+        request: ens_20171110_models.DescribeAICImagesRequest,
+    ) -> ens_20171110_models.DescribeAICImagesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_aicimages_with_options_async(request, runtime)
+
     def describe_armserver_instances_with_options(
         self,
         tmp_req: ens_20171110_models.DescribeARMServerInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ens_20171110_models.DescribeARMServerInstancesResponse:
         UtilClient.validate_model(tmp_req)
         request = ens_20171110_models.DescribeARMServerInstancesShrinkRequest()
@@ -7125,14 +7207,80 @@
     async def describe_export_image_status_async(
         self,
         request: ens_20171110_models.DescribeExportImageStatusRequest,
     ) -> ens_20171110_models.DescribeExportImageStatusResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_export_image_status_with_options_async(request, runtime)
 
+    def describe_file_systems_with_options(
+        self,
+        request: ens_20171110_models.DescribeFileSystemsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ens_20171110_models.DescribeFileSystemsResponse:
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
+    async def describe_file_systems_with_options_async(
+        self,
+        request: ens_20171110_models.DescribeFileSystemsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ens_20171110_models.DescribeFileSystemsResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_file_systems(
+        self,
+        request: ens_20171110_models.DescribeFileSystemsRequest,
+    ) -> ens_20171110_models.DescribeFileSystemsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_file_systems_with_options(request, runtime)
+
+    async def describe_file_systems_async(
+        self,
+        request: ens_20171110_models.DescribeFileSystemsRequest,
+    ) -> ens_20171110_models.DescribeFileSystemsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_file_systems_with_options_async(request, runtime)
+
     def describe_forward_table_entries_with_options(
         self,
         request: ens_20171110_models.DescribeForwardTableEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ens_20171110_models.DescribeForwardTableEntriesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7874,14 +8022,16 @@
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
@@ -7932,14 +8082,16 @@
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
@@ -9118,16 +9270,14 @@
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
@@ -9154,16 +9304,14 @@
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
@@ -9836,16 +9984,14 @@
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
@@ -9876,16 +10022,14 @@
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

### Comparing `alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110/models.py` & `alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7622,14 +7622,195 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteVSwitchResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeAICImagesRequest(TeaModel):
+    def __init__(
+        self,
+        image_id: str = None,
+        image_url: str = None,
+        page_number: str = None,
+        page_size: str = None,
+    ):
+        self.image_id = image_id
+        self.image_url = image_url
+        self.page_number = page_number
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        creation_time: str = None,
+        image_id: str = None,
+        image_url: str = None,
+        status: str = None,
+        user: str = None,
+    ):
+        self.creation_time = creation_time
+        self.image_id = image_id
+        self.image_url = image_url
+        self.status = status
+        self.user = user
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        images: List[DescribeAICImagesResponseBodyImages] = None,
+        request_id: str = None,
+    ):
+        self.images = images
+        self.request_id = request_id
+
+    def validate(self):
+        if self.images:
+            for k in self.images:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeAICImagesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         ens_region_ids: List[str] = None,
         page_number: int = None,
         page_size: int = None,
         server_ids: List[str] = None,
@@ -15609,14 +15790,308 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeExportImageStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeFileSystemsRequest(TeaModel):
+    def __init__(
+        self,
+        ens_region_id: str = None,
+        file_system_id: str = None,
+        file_system_name: str = None,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        self.ens_region_id = ens_region_id
+        self.file_system_id = file_system_id
+        self.file_system_name = file_system_name
+        self.page_number = page_number
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        mount_target_domain: str = None,
+        mount_target_name: str = None,
+        net_work_id: str = None,
+        status: str = None,
+    ):
+        self.mount_target_domain = mount_target_domain
+        self.mount_target_name = mount_target_name
+        self.net_work_id = net_work_id
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        capacity: int = None,
+        creation_time: str = None,
+        ens_region_id: str = None,
+        file_system_id: str = None,
+        file_system_name: str = None,
+        metered_size: int = None,
+        mount_targets: List[DescribeFileSystemsResponseBodyFileSystemsMountTargets] = None,
+        pay_type: str = None,
+        protocol_type: str = None,
+        status: str = None,
+        storage_type: str = None,
+    ):
+        self.capacity = capacity
+        self.creation_time = creation_time
+        self.ens_region_id = ens_region_id
+        self.file_system_id = file_system_id
+        self.file_system_name = file_system_name
+        self.metered_size = metered_size
+        self.mount_targets = mount_targets
+        self.pay_type = pay_type
+        self.protocol_type = protocol_type
+        self.status = status
+        self.storage_type = storage_type
+
+    def validate(self):
+        if self.mount_targets:
+            for k in self.mount_targets:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        file_systems: List[DescribeFileSystemsResponseBodyFileSystems] = None,
+        page_number: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.file_systems = file_systems
+        self.page_number = page_number
+        self.page_size = page_size
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.file_systems:
+            for k in self.file_systems:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeFileSystemsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         external_ip: str = None,
         forward_entry_id: str = None,
         forward_entry_name: str = None,
         internal_ip: str = None,
@@ -17448,14 +17923,15 @@
         ens_region_ids: str = None,
         ens_service_id: str = None,
         image_id: str = None,
         instance_id: str = None,
         instance_ids: str = None,
         instance_name: str = None,
         instance_resource_type: str = None,
+        intranet_ip: str = None,
         network_id: str = None,
         order_by_params: str = None,
         page_number: int = None,
         page_size: str = None,
         search_key: str = None,
         security_group_id: str = None,
         status: str = None,
@@ -17465,14 +17941,15 @@
         self.ens_region_ids = ens_region_ids
         self.ens_service_id = ens_service_id
         self.image_id = image_id
         self.instance_id = instance_id
         self.instance_ids = instance_ids
         self.instance_name = instance_name
         self.instance_resource_type = instance_resource_type
+        self.intranet_ip = intranet_ip
         self.network_id = network_id
         self.order_by_params = order_by_params
         self.page_number = page_number
         self.page_size = page_size
         self.search_key = search_key
         self.security_group_id = security_group_id
         self.status = status
@@ -17499,14 +17976,16 @@
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
@@ -17535,14 +18014,16 @@
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
@@ -22419,21 +22900,19 @@
 class DescribePrePaidInstanceStockRequest(TeaModel):
     def __init__(
         self,
         data_disk_size: int = None,
         ens_region_id: str = None,
         instance_spec: str = None,
         system_disk_size: int = None,
-        version: str = None,
     ):
         self.data_disk_size = data_disk_size
         self.ens_region_id = ens_region_id
         self.instance_spec = instance_spec
         self.system_disk_size = system_disk_size
-        self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -22444,52 +22923,50 @@
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         avaliable_count: int = None,
         cores: int = None,
         data_disk_size: int = None,
         ens_region_id: str = None,
         instance_spec: str = None,
         memory: int = None,
         request_id: str = None,
+        resource_gap: str = None,
         system_disk_size: int = None,
     ):
         self.avaliable_count = avaliable_count
         self.cores = cores
         self.data_disk_size = data_disk_size
         self.ens_region_id = ens_region_id
         self.instance_spec = instance_spec
         self.memory = memory
         self.request_id = request_id
+        self.resource_gap = resource_gap
         self.system_disk_size = system_disk_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22507,14 +22984,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AvaliableCount') is not None:
@@ -22527,14 +23006,16 @@
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
     def __init__(
@@ -24763,23 +25244,21 @@
         self,
         end_time: str = None,
         ens_region_id: str = None,
         instance_id: str = None,
         isp: str = None,
         period: str = None,
         start_time: str = None,
-        version: str = None,
     ):
         self.end_time = end_time
         self.ens_region_id = ens_region_id
         self.instance_id = instance_id
         self.isp = isp
         self.period = period
         self.start_time = start_time
-        self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -24794,16 +25273,14 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('EnsRegionId') is not None:
@@ -24812,16 +25289,14 @@
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
     def __init__(
         self,
         down_band_width: int = None,
```

### Comparing `alibabacloud_ens20171110-3.0.8/alibabacloud_ens20171110.egg-info/PKG-INFO` & `alibabacloud_ens20171110-3.0.9/alibabacloud_ens20171110.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ens20171110
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud edge node service (20171110) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ens20171110-3.0.8/setup.py` & `alibabacloud_ens20171110-3.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ens20171110.
 
-Created on 22/09/2022
+Created on 13/10/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ens20171110"
 NAME = "alibabacloud_ens20171110" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud edge node service (20171110) SDK Library for Python"
```

