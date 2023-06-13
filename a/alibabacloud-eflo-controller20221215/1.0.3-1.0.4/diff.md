# Comparing `tmp/alibabacloud_eflo-controller20221215-1.0.3.tar.gz` & `tmp/alibabacloud_eflo-controller20221215-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eflo-controller20221215-1.0.3.tar", last modified: Mon Apr 24 08:13:43 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eflo-controller20221215-1.0.4.tar", last modified: Tue Jun 13 02:39:31 2023, max compression
```

## Comparing `alibabacloud_eflo-controller20221215-1.0.3.tar` & `alibabacloud_eflo-controller20221215-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62687 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/client.py
--rw-r--r--   0 root         (0) root         (0)   146540 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2672 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62687 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215/client.py
+-rw-r--r--   0 root         (0) root         (0)   146885 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-06-13 02:39:31.000000 alibabacloud_eflo-controller20221215-1.0.4/setup.py
```

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/LICENSE` & `alibabacloud_eflo-controller20221215-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/PKG-INFO` & `alibabacloud_eflo-controller20221215-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eflo-controller20221215
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/README-CN.md` & `alibabacloud_eflo-controller20221215-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/README.md` & `alibabacloud_eflo-controller20221215-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/client.py` & `alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/models.py` & `alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,15 +576,17 @@
 
 class CreateClusterRequestNetworksVpdInfo(TeaModel):
     def __init__(
         self,
         vpd_id: str = None,
         vpd_subnets: List[str] = None,
     ):
+        # 专有网络 id
         self.vpd_id = vpd_id
+        # 集群子网id列表
         self.vpd_subnets = vpd_subnets
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -612,14 +614,15 @@
         self,
         ip_allocation_policy: List[CreateClusterRequestNetworksIpAllocationPolicy] = None,
         new_vpd_info: CreateClusterRequestNetworksNewVpdInfo = None,
         vpd_info: CreateClusterRequestNetworksVpdInfo = None,
     ):
         self.ip_allocation_policy = ip_allocation_policy
         self.new_vpd_info = new_vpd_info
+        # 复用VPD信息
         self.vpd_info = vpd_info
 
     def validate(self):
         if self.ip_allocation_policy:
             for k in self.ip_allocation_policy:
                 if k:
                     k.validate()
@@ -1545,14 +1548,15 @@
     ):
         self.cluster_id = cluster_id
         self.cluster_name = cluster_name
         self.create_time = create_time
         self.expired_time = expired_time
         self.hostname = hostname
         self.image_id = image_id
+        # 镜像名称
         self.image_name = image_name
         self.machine_type = machine_type
         self.networks = networks
         self.node_group_id = node_group_id
         self.node_group_name = node_group_name
         self.node_id = node_id
         self.operating_state = operating_state
@@ -2001,24 +2005,26 @@
 class DescribeTaskResponseBody(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         cluster_name: str = None,
         create_time: str = None,
         message: str = None,
+        node_ids: List[str] = None,
         request_id: str = None,
         steps: List[DescribeTaskResponseBodySteps] = None,
         task_state: str = None,
         task_type: str = None,
         update_time: str = None,
     ):
         self.cluster_id = cluster_id
         self.cluster_name = cluster_name
         self.create_time = create_time
         self.message = message
+        self.node_ids = node_ids
         self.request_id = request_id
         self.steps = steps
         self.task_state = task_state
         self.task_type = task_type
         self.update_time = update_time
 
     def validate(self):
@@ -2037,14 +2043,16 @@
             result['ClusterId'] = self.cluster_id
         if self.cluster_name is not None:
             result['ClusterName'] = self.cluster_name
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.message is not None:
             result['Message'] = self.message
+        if self.node_ids is not None:
+            result['NodeIds'] = self.node_ids
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         result['Steps'] = []
         if self.steps is not None:
             for k in self.steps:
                 result['Steps'].append(k.to_map() if k else None)
         if self.task_state is not None:
@@ -2061,14 +2069,16 @@
             self.cluster_id = m.get('ClusterId')
         if m.get('ClusterName') is not None:
             self.cluster_name = m.get('ClusterName')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('Message') is not None:
             self.message = m.get('Message')
+        if m.get('NodeIds') is not None:
+            self.node_ids = m.get('NodeIds')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         self.steps = []
         if m.get('Steps') is not None:
             for k in m.get('Steps'):
                 temp_model = DescribeTaskResponseBodySteps()
                 self.steps.append(temp_model.from_map(k))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/PKG-INFO` & `alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eflo-controller20221215
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/SOURCES.txt` & `alibabacloud_eflo-controller20221215-1.0.4/alibabacloud_eflo_controller20221215.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.3/setup.py` & `alibabacloud_eflo-controller20221215-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eflo-controller20221215.
 
-Created on 24/04/2023
+Created on 13/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eflo_controller20221215"
 NAME = "alibabacloud_eflo-controller20221215" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eflo-controller (20221215) SDK Library for Python"
```

