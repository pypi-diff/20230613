# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.911.tar", last modified: Fri Jun  9 02:19:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.912.tar", last modified: Mon Jun 12 03:03:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.911.tar` & `tencentcloud-sdk-python-essbasic-3.0.912.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16533 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51697 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   234715 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51715 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   234732 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:03:42.000000 tencentcloud-sdk-python-essbasic-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,17 @@
 
 # 类型不支持。
 INVALIDPARAMETER_SIGNCOMPONENTS = 'InvalidParameter.SignComponents'
 
 # 状态异常。
 INVALIDPARAMETER_STATUS = 'InvalidParameter.Status'
 
+# 统一社会信用代码不符合要求
+INVALIDPARAMETER_UNIFORMSOCIALCREDITCODE = 'InvalidParameter.UniformSocialCreditCode'
+
 # 参数错误，不合法的签署顺序，请检查后重试。
 INVALIDPARAMETER_UNORDERED = 'InvalidParameter.Unordered'
 
 # 参数错误，不支持的控件类型，请检查后重试。
 INVALIDPARAMETER_UNSUPPORTEDCOMPONENTTYPE = 'InvalidParameter.UnsupportedComponentType'
 
 # 流程id不存在。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelCreateConvertTaskApi(self, request):
-        """上传了word、excel文件后，通过该接口发起文件转换任务，将word、excel文件转换为pdf文件。
+        """上传了word、excel、图片文件后，通过该接口发起文件转换任务，将word、excel、图片文件转换为pdf文件。
 
         :param request: Request instance for ChannelCreateConvertTaskApi.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateConvertTaskApiRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateConvertTaskApiResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,15 +596,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
-        :param ResourceType: 资源类型 取值范围doc,docx,html,xls,xlsx之一
+        :param ResourceType: 资源类型 支持doc,docx,html,xls,xlsx,jpg,jpeg,png,bmp文件类型
         :type ResourceType: str
         :param ResourceName: 资源名称，长度限制为256字符
         :type ResourceName: str
         :param ResourceId: 资源Id，通过UploadFiles获取
         :type ResourceId: str
         :param Operator: 调用方用户信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.912/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.911/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.912/setup.py`

 * *Files identical despite different names*

