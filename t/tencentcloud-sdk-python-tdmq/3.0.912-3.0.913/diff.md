# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.912.tar", last modified: Mon Jun 12 03:13:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.913.tar", last modified: Tue Jun 13 02:26:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.912.tar` & `tencentcloud-sdk-python-tdmq-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   103792 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   385664 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:13:25.000000 tencentcloud-sdk-python-tdmq-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   110188 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   405083 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.912/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -847,14 +847,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteRabbitMQUser(self, request):
+        """删除RabbitMQ的用户
+
+        :param request: Request instance for DeleteRabbitMQUser.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQUserRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQUserResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteRabbitMQUser", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteRabbitMQUserResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteRabbitMQVirtualHost(self, request):
+        """删除RabbitMQ的vhost
+
+        :param request: Request instance for DeleteRabbitMQVirtualHost.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQVirtualHostRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQVirtualHostResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteRabbitMQVirtualHost", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteRabbitMQVirtualHostResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteRocketMQCluster(self, request):
         """删除RocketMQ集群
 
         :param request: Request instance for DeleteRocketMQCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRocketMQClusterRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.DeleteRocketMQClusterResponse`
 
@@ -1664,14 +1710,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeRabbitMQUser(self, request):
+        """查询RabbitMQ用户列表
+
+        :param request: Request instance for DescribeRabbitMQUser.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQUserRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQUserResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeRabbitMQUser", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeRabbitMQUserResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeRabbitMQVipInstance(self, request):
         """获取单个RabbitMQ专享实例信息
 
         :param request: Request instance for DescribeRabbitMQVipInstance.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVipInstanceRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVipInstanceResponse`
 
@@ -1710,14 +1779,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeRabbitMQVirtualHost(self, request):
+        """查询RabbitMQ vhost列表
+
+        :param request: Request instance for DescribeRabbitMQVirtualHost.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVirtualHostRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVirtualHostResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeRabbitMQVirtualHost", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeRabbitMQVirtualHostResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeRabbitMQVirtualHostList(self, request):
+        """RabbitMQ专享版查询虚拟主机列表
+
+        :param request: Request instance for DescribeRabbitMQVirtualHostList.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVirtualHostListRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVirtualHostListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeRabbitMQVirtualHostList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeRabbitMQVirtualHostListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeRocketMQCluster(self, request):
         """获取单个RocketMQ集群信息
 
         :param request: Request instance for DescribeRocketMQCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQClusterRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQClusterResponse`
 
@@ -2199,14 +2314,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyRabbitMQUser(self, request):
+        """修改RabbitMQ的用户
+
+        :param request: Request instance for ModifyRabbitMQUser.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQUserRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQUserResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyRabbitMQUser", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyRabbitMQUserResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyRabbitMQVipInstance(self, request):
         """修改RabbitMQ专享版实例
 
         :param request: Request instance for ModifyRabbitMQVipInstance.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQVipInstanceRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQVipInstanceResponse`
 
@@ -2220,14 +2358,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyRabbitMQVirtualHost(self, request):
+        """修改RabbitMQ的vhost
+
+        :param request: Request instance for ModifyRabbitMQVirtualHost.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQVirtualHostRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQVirtualHostResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyRabbitMQVirtualHost", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyRabbitMQVirtualHostResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyRocketMQCluster(self, request):
         """更新RocketMQ集群信息
 
         :param request: Request instance for ModifyRocketMQCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQClusterRequest`
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3293,14 +3293,104 @@
 
 
     def _deserialize(self, params):
         self.EnvironmentIds = params.get("EnvironmentIds")
         self.RequestId = params.get("RequestId")
 
 
+class DeleteRabbitMQUserRequest(AbstractModel):
+    """DeleteRabbitMQUser请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群实例Id
+        :type InstanceId: str
+        :param User: 用户名，登录时使用
+        :type User: str
+        """
+        self.InstanceId = None
+        self.User = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.User = params.get("User")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteRabbitMQUserResponse(AbstractModel):
+    """DeleteRabbitMQUser返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class DeleteRabbitMQVirtualHostRequest(AbstractModel):
+    """DeleteRabbitMQVirtualHost请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群实例Id
+        :type InstanceId: str
+        :param VirtualHost: vhost名
+        :type VirtualHost: str
+        """
+        self.InstanceId = None
+        self.VirtualHost = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.VirtualHost = params.get("VirtualHost")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteRabbitMQVirtualHostResponse(AbstractModel):
+    """DeleteRabbitMQVirtualHost返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteRocketMQClusterRequest(AbstractModel):
     """DeleteRocketMQCluster请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5588,14 +5678,88 @@
             for item in params.get("NodeList"):
                 obj = RabbitMQPrivateNode()
                 obj._deserialize(item)
                 self.NodeList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeRabbitMQUserRequest(AbstractModel):
+    """DescribeRabbitMQUser请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群实例Id
+        :type InstanceId: str
+        :param SearchUser: 用户名检索，支持前缀匹配，后缀匹配
+        :type SearchUser: str
+        :param Offset: 分页Offset
+        :type Offset: int
+        :param Limit: 分页Limit
+        :type Limit: int
+        :param User: 用户名，精确查询
+        :type User: str
+        :param Tags: 用户标签，根据标签过滤列表
+        :type Tags: list of str
+        """
+        self.InstanceId = None
+        self.SearchUser = None
+        self.Offset = None
+        self.Limit = None
+        self.User = None
+        self.Tags = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.SearchUser = params.get("SearchUser")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.User = params.get("User")
+        self.Tags = params.get("Tags")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRabbitMQUserResponse(AbstractModel):
+    """DescribeRabbitMQUser返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 返回的User数量
+        :type TotalCount: int
+        :param RabbitMQUserList: 当前已创建的RabbitMQ用户列表
+        :type RabbitMQUserList: list of RabbitMQUser
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.RabbitMQUserList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("RabbitMQUserList") is not None:
+            self.RabbitMQUserList = []
+            for item in params.get("RabbitMQUserList"):
+                obj = RabbitMQUser()
+                obj._deserialize(item)
+                self.RabbitMQUserList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeRabbitMQVipInstanceRequest(AbstractModel):
     """DescribeRabbitMQVipInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5740,14 +5904,149 @@
             for item in params.get("Instances"):
                 obj = RabbitMQVipInstance()
                 obj._deserialize(item)
                 self.Instances.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeRabbitMQVirtualHostListRequest(AbstractModel):
+    """DescribeRabbitMQVirtualHostList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 不适用，默认参数
+        :type InstanceId: str
+        :param Offset: 偏移量
+        :type Offset: int
+        :param Limit: 一页限制
+        :type Limit: int
+        """
+        self.InstanceId = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRabbitMQVirtualHostListResponse(AbstractModel):
+    """DescribeRabbitMQVirtualHostList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 集群列表数量
+        :type TotalCount: int
+        :param VirtualHostList: 集群列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VirtualHostList: list of RabbitMQPrivateVirtualHost
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.VirtualHostList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("VirtualHostList") is not None:
+            self.VirtualHostList = []
+            for item in params.get("VirtualHostList"):
+                obj = RabbitMQPrivateVirtualHost()
+                obj._deserialize(item)
+                self.VirtualHostList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeRabbitMQVirtualHostRequest(AbstractModel):
+    """DescribeRabbitMQVirtualHost请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群实例Id
+        :type InstanceId: str
+        :param VirtualHost: vhost名,不传则查询全部
+        :type VirtualHost: str
+        :param Offset: 分页Offset
+        :type Offset: int
+        :param Limit: 分页Limit
+        :type Limit: int
+        :param Filters: search-virtual-host：vhost名称模糊查询，之前前缀和后缀匹配
+        :type Filters: :class:`tencentcloud.tdmq.v20200217.models.Filter`
+        """
+        self.InstanceId = None
+        self.VirtualHost = None
+        self.Offset = None
+        self.Limit = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.VirtualHost = params.get("VirtualHost")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        if params.get("Filters") is not None:
+            self.Filters = Filter()
+            self.Filters._deserialize(params.get("Filters"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRabbitMQVirtualHostResponse(AbstractModel):
+    """DescribeRabbitMQVirtualHost返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 返回vhost数量
+        :type TotalCount: int
+        :param VirtualHostList: vhost详情列表
+        :type VirtualHostList: list of RabbitMQVirtualHostInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.VirtualHostList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("VirtualHostList") is not None:
+            self.VirtualHostList = []
+            for item in params.get("VirtualHostList"):
+                obj = RabbitMQVirtualHostInfo()
+                obj._deserialize(item)
+                self.VirtualHostList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeRocketMQClusterRequest(AbstractModel):
     """DescribeRocketMQCluster请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7563,14 +7862,79 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyRabbitMQUserRequest(AbstractModel):
+    """ModifyRabbitMQUser请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群实例Id
+        :type InstanceId: str
+        :param User: 用户名，登录时使用
+        :type User: str
+        :param Password: 密码，登录时使用
+        :type Password: str
+        :param Description: 描述，不传则不修改
+        :type Description: str
+        :param Tags: 用户标签，用于决定改用户访问RabbitMQ Management的权限范围，不传则不修改
+        :type Tags: list of str
+        :param MaxConnections: 该用户的最大连接数，不传则不修改
+        :type MaxConnections: int
+        :param MaxChannels: 该用户的最大channel数，不传则不修改
+        :type MaxChannels: int
+        """
+        self.InstanceId = None
+        self.User = None
+        self.Password = None
+        self.Description = None
+        self.Tags = None
+        self.MaxConnections = None
+        self.MaxChannels = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.User = params.get("User")
+        self.Password = params.get("Password")
+        self.Description = params.get("Description")
+        self.Tags = params.get("Tags")
+        self.MaxConnections = params.get("MaxConnections")
+        self.MaxChannels = params.get("MaxChannels")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyRabbitMQUserResponse(AbstractModel):
+    """ModifyRabbitMQUser返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyRabbitMQVipInstanceRequest(AbstractModel):
     """ModifyRabbitMQVipInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7617,14 +7981,67 @@
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.RequestId = params.get("RequestId")
 
 
+class ModifyRabbitMQVirtualHostRequest(AbstractModel):
+    """ModifyRabbitMQVirtualHost请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群实例Id
+        :type InstanceId: str
+        :param VirtualHost: vhost名
+        :type VirtualHost: str
+        :param Description: 描述
+        :type Description: str
+        :param TraceFlag: 消息轨迹开关,true打开,false关闭
+        :type TraceFlag: bool
+        """
+        self.InstanceId = None
+        self.VirtualHost = None
+        self.Description = None
+        self.TraceFlag = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.VirtualHost = params.get("VirtualHost")
+        self.Description = params.get("Description")
+        self.TraceFlag = params.get("TraceFlag")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyRabbitMQVirtualHostResponse(AbstractModel):
+    """ModifyRabbitMQVirtualHost返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyRocketMQClusterRequest(AbstractModel):
     """ModifyRocketMQCluster请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8859,14 +9276,98 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RabbitMQPrivateVirtualHost(AbstractModel):
+    """RabbitMQ专享版虚拟机
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VirtualHostName: 虚拟主机的名字
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VirtualHostName: str
+        :param Description: 虚拟主机的描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        """
+        self.VirtualHostName = None
+        self.Description = None
+
+
+    def _deserialize(self, params):
+        self.VirtualHostName = params.get("VirtualHostName")
+        self.Description = params.get("Description")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RabbitMQUser(AbstractModel):
+    """RabbitMQ用户实体详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群实例Id
+        :type InstanceId: str
+        :param User: 用户名，登录时使用
+        :type User: str
+        :param Password: 密码，登录时使用
+        :type Password: str
+        :param Description: 用户描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param Tags: 用户标签，用于决定改用户访问RabbitMQ Management的权限范围
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of str
+        :param CreateTime: 用户创建时间
+        :type CreateTime: str
+        :param ModifyTime: 用户最后修改时间
+        :type ModifyTime: str
+        :param Type: 用户类型，System：系统创建，User：用户创建
+        :type Type: str
+        """
+        self.InstanceId = None
+        self.User = None
+        self.Password = None
+        self.Description = None
+        self.Tags = None
+        self.CreateTime = None
+        self.ModifyTime = None
+        self.Type = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.User = params.get("User")
+        self.Password = params.get("Password")
+        self.Description = params.get("Description")
+        self.Tags = params.get("Tags")
+        self.CreateTime = params.get("CreateTime")
+        self.ModifyTime = params.get("ModifyTime")
+        self.Type = params.get("Type")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class RabbitMQVipInstance(AbstractModel):
     """RabbitMQ专享实例信息
 
     """
 
     def __init__(self):
         r"""
@@ -8945,14 +9446,109 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class RabbitMQVirtualHostInfo(AbstractModel):
+    """RabbitMQ的vhost详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 集群实例Id
+        :type InstanceId: str
+        :param VirtualHost: vhost名
+        :type VirtualHost: str
+        :param Description: vhost描述信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param Tags: vhost标签
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of str
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param ModifyTime: 修改时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModifyTime: str
+        :param VirtualHostStatistics: vhost概览统计信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VirtualHostStatistics: :class:`tencentcloud.tdmq.v20200217.models.RabbitMQVirtualHostStatistics`
+        """
+        self.InstanceId = None
+        self.VirtualHost = None
+        self.Description = None
+        self.Tags = None
+        self.CreateTime = None
+        self.ModifyTime = None
+        self.VirtualHostStatistics = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.VirtualHost = params.get("VirtualHost")
+        self.Description = params.get("Description")
+        self.Tags = params.get("Tags")
+        self.CreateTime = params.get("CreateTime")
+        self.ModifyTime = params.get("ModifyTime")
+        if params.get("VirtualHostStatistics") is not None:
+            self.VirtualHostStatistics = RabbitMQVirtualHostStatistics()
+            self.VirtualHostStatistics._deserialize(params.get("VirtualHostStatistics"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RabbitMQVirtualHostStatistics(AbstractModel):
+    """vhost概览统计信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CurrentQueues: 当前vhost的queue数量
+        :type CurrentQueues: int
+        :param CurrentExchanges: 当前vhost的exchange数量
+        :type CurrentExchanges: int
+        :param CurrentConnections: 当前vhost的连接数量
+        :type CurrentConnections: int
+        :param CurrentChannels: 当前vhost的channel数量
+        :type CurrentChannels: int
+        :param CurrentUsers: 当前vhost的用户数量
+        :type CurrentUsers: int
+        """
+        self.CurrentQueues = None
+        self.CurrentExchanges = None
+        self.CurrentConnections = None
+        self.CurrentChannels = None
+        self.CurrentUsers = None
+
+
+    def _deserialize(self, params):
+        self.CurrentQueues = params.get("CurrentQueues")
+        self.CurrentExchanges = params.get("CurrentExchanges")
+        self.CurrentConnections = params.get("CurrentConnections")
+        self.CurrentChannels = params.get("CurrentChannels")
+        self.CurrentUsers = params.get("CurrentUsers")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class ReceiveMessageRequest(AbstractModel):
     """ReceiveMessage请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.912'
+__version__ = '3.0.913'
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.913/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.912/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.912/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.913/setup.py`

 * *Files identical despite different names*

