# Comparing `tmp/alibabacloud_eflo-controller20221215_py2-1.0.3.tar.gz` & `tmp/alibabacloud_eflo-controller20221215_py2-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eflo-controller20221215_py2-1.0.3.tar", last modified: Mon Apr 24 08:13:20 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eflo-controller20221215_py2-1.0.4.tar", last modified: Tue Jun 13 02:38:45 2023, max compression
```

## Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3.tar` & `alibabacloud_eflo-controller20221215_py2-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2544 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1069 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1152 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26047 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/client.py
--rw-r--r--   0 root         (0) root         (0)   147475 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2544 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      536 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2965 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26047 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215/client.py
+-rw-r--r--   0 root         (0) root         (0)   147818 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      536 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-06-13 02:38:45.000000 alibabacloud_eflo-controller20221215_py2-1.0.4/setup.py
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/LICENSE` & `alibabacloud_eflo-controller20221215_py2-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/PKG-INFO` & `alibabacloud_eflo-controller20221215_py2-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eflo-controller20221215_py2
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/README-CN.md` & `alibabacloud_eflo-controller20221215_py2-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/README.md` & `alibabacloud_eflo-controller20221215_py2-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/client.py` & `alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/models.py` & `alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,15 +508,17 @@
                 temp_model = CreateClusterRequestNetworksNewVpdInfoVpdSubnets()
                 self.vpd_subnets.append(temp_model.from_map(k))
         return self
 
 
 class CreateClusterRequestNetworksVpdInfo(TeaModel):
     def __init__(self, vpd_id=None, vpd_subnets=None):
+        # 专有网络 id
         self.vpd_id = vpd_id  # type: str
+        # 集群子网id列表
         self.vpd_subnets = vpd_subnets  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateClusterRequestNetworksVpdInfo, self).to_map()
@@ -539,14 +541,15 @@
         return self
 
 
 class CreateClusterRequestNetworks(TeaModel):
     def __init__(self, ip_allocation_policy=None, new_vpd_info=None, vpd_info=None):
         self.ip_allocation_policy = ip_allocation_policy  # type: list[CreateClusterRequestNetworksIpAllocationPolicy]
         self.new_vpd_info = new_vpd_info  # type: CreateClusterRequestNetworksNewVpdInfo
+        # 复用VPD信息
         self.vpd_info = vpd_info  # type: CreateClusterRequestNetworksVpdInfo
 
     def validate(self):
         if self.ip_allocation_policy:
             for k in self.ip_allocation_policy:
                 if k:
                     k.validate()
@@ -1357,14 +1360,15 @@
                  node_id=None, operating_state=None, request_id=None, sn=None, zone_id=None):
         self.cluster_id = cluster_id  # type: str
         self.cluster_name = cluster_name  # type: str
         self.create_time = create_time  # type: str
         self.expired_time = expired_time  # type: str
         self.hostname = hostname  # type: str
         self.image_id = image_id  # type: str
+        # 镜像名称
         self.image_name = image_name  # type: str
         self.machine_type = machine_type  # type: str
         self.networks = networks  # type: list[DescribeNodeResponseBodyNetworks]
         self.node_group_id = node_group_id  # type: str
         self.node_group_name = node_group_name  # type: str
         self.node_id = node_id  # type: str
         self.operating_state = operating_state  # type: str
@@ -1767,20 +1771,21 @@
                 self.sub_tasks.append(temp_model.from_map(k))
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class DescribeTaskResponseBody(TeaModel):
-    def __init__(self, cluster_id=None, cluster_name=None, create_time=None, message=None, request_id=None,
-                 steps=None, task_state=None, task_type=None, update_time=None):
+    def __init__(self, cluster_id=None, cluster_name=None, create_time=None, message=None, node_ids=None,
+                 request_id=None, steps=None, task_state=None, task_type=None, update_time=None):
         self.cluster_id = cluster_id  # type: str
         self.cluster_name = cluster_name  # type: str
         self.create_time = create_time  # type: str
         self.message = message  # type: str
+        self.node_ids = node_ids  # type: list[str]
         self.request_id = request_id  # type: str
         self.steps = steps  # type: list[DescribeTaskResponseBodySteps]
         self.task_state = task_state  # type: str
         self.task_type = task_type  # type: str
         self.update_time = update_time  # type: str
 
     def validate(self):
@@ -1799,14 +1804,16 @@
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
@@ -1823,14 +1830,16 @@
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

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO` & `alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eflo-controller20221215-py2
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt` & `alibabacloud_eflo-controller20221215_py2-1.0.4/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.3/setup.py` & `alibabacloud_eflo-controller20221215_py2-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eflo-controller20221215_py2.
 
-Created on 24/04/2023
+Created on 13/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eflo_controller20221215"
 NAME = "alibabacloud_eflo-controller20221215_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eflo-controller (20221215) SDK Library for Python2"
```

