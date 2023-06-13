# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.911.tar", last modified: Fri Jun  9 02:14:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.912.tar", last modified: Mon Jun 12 02:59:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.911.tar` & `tencentcloud-sdk-python-cfw-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:14:56.000000 tencentcloud-sdk-python-cfw-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-09 02:14:56.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    66476 2023-06-09 02:14:56.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:14:56.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223771 2023-06-09 02:14:56.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:14:56.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:14:56.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:14:56.000000 tencentcloud-sdk-python-cfw-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:14:57.000000 tencentcloud-sdk-python-cfw-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    67446 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   224528 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 02:59:14.000000 tencentcloud-sdk-python-cfw-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.911/README.rst` & `tencentcloud-sdk-python-cfw-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,14 +528,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeEnterpriseSGRuleProgress(self, request):
+        """查询新版安全组下发进度
+
+        :param request: Request instance for DescribeEnterpriseSGRuleProgress.
+        :type request: :class:`tencentcloud.cfw.v20190904.models.DescribeEnterpriseSGRuleProgressRequest`
+        :rtype: :class:`tencentcloud.cfw.v20190904.models.DescribeEnterpriseSGRuleProgressResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeEnterpriseSGRuleProgress", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeEnterpriseSGRuleProgressResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeEnterpriseSecurityGroupRule(self, request):
         """查询新企业安全组规则
 
         :param request: Request instance for DescribeEnterpriseSecurityGroupRule.
         :type request: :class:`tencentcloud.cfw.v20190904.models.DescribeEnterpriseSecurityGroupRuleRequest`
         :rtype: :class:`tencentcloud.cfw.v20190904.models.DescribeEnterpriseSecurityGroupRuleResponse`
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/cfw/v20190904/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2194,14 +2194,41 @@
         self.VirtualPatchSwitch = params.get("VirtualPatchSwitch")
         self.HistoryOpen = params.get("HistoryOpen")
         self.ReturnCode = params.get("ReturnCode")
         self.ReturnMsg = params.get("ReturnMsg")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeEnterpriseSGRuleProgressRequest(AbstractModel):
+    """DescribeEnterpriseSGRuleProgress请求参数结构体
+
+    """
+
+
+class DescribeEnterpriseSGRuleProgressResponse(AbstractModel):
+    """DescribeEnterpriseSGRuleProgress返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Progress: 0-100，代表下发进度百分比
+        :type Progress: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Progress = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Progress = params.get("Progress")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeEnterpriseSecurityGroupRuleRequest(AbstractModel):
     """DescribeEnterpriseSecurityGroupRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.912/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.911'
+__version__ = '3.0.912'
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.911/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.912/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.911/setup.py` & `tencentcloud-sdk-python-cfw-3.0.912/setup.py`

 * *Files identical despite different names*

