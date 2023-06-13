# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.912.tar", last modified: Mon Jun 12 02:56:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.913.tar", last modified: Tue Jun 13 02:03:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.912.tar` & `tencentcloud-sdk-python-autoscaling-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)    60396 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)    19836 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258492 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 02:56:33.000000 tencentcloud-sdk-python-autoscaling-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)    60526 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)    19836 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258716 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:03:59.000000 tencentcloud-sdk-python-autoscaling-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1154,14 +1154,15 @@
 
     def ScaleOutInstances(self, request):
         """为伸缩组指定数量扩容实例，返回扩容活动的 ActivityId。
         * 伸缩组需要未处于活动中
         * 伸缩组处于停用状态时，该接口也会生效，可参考[停用伸缩组](https://cloud.tencent.com/document/api/377/20435)文档查看伸缩组停用状态的影响范围
         * 接口会增加期望实例数，新的期望实例数需要小于等于最大实例数
         * 扩容如果失败或者部分成功，最后期望实例数只会增加实际成功的实例数量
+        * 竞价混合模式中一次扩容可能触发多个伸缩活动，该接口仅返回第一个伸缩活动的 ActivityId
 
         :param request: Request instance for ScaleOutInstances.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.ScaleOutInstancesRequest`
         :rtype: :class:`tencentcloud.autoscaling.v20180419.models.ScaleOutInstancesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/autoscaling/v20180419/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,24 +169,30 @@
         r"""
         :param Problem: 问题描述。
         :type Problem: str
         :param Detail: 问题详情。
         :type Detail: str
         :param Solution: 建议解决方案。
         :type Solution: str
+        :param Level: 伸缩建议警告级别。取值范围：<br>
+<li>WARNING：警告级别<br>
+<li>CRITICAL：严重级别<br>
+        :type Level: str
         """
         self.Problem = None
         self.Detail = None
         self.Solution = None
+        self.Level = None
 
 
     def _deserialize(self, params):
         self.Problem = params.get("Problem")
         self.Detail = params.get("Detail")
         self.Solution = params.get("Solution")
+        self.Level = params.get("Level")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.913/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.913/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.912/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.913/setup.py`

 * *Files identical despite different names*

