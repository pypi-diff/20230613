# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.912.tar", last modified: Mon Jun 12 03:02:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.913.tar", last modified: Tue Jun 13 02:09:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.912.tar` & `tencentcloud-sdk-python-dnspod-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-12 03:02:11.000000 tencentcloud-sdk-python-dnspod-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    23568 2023-06-12 03:02:11.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:02:11.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   209672 2023-06-12 03:02:11.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    59836 2023-06-12 03:02:11.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:02:11.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:02:11.000000 tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-12 03:02:11.000000 tencentcloud-sdk-python-dnspod-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:02:12.000000 tencentcloud-sdk-python-dnspod-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    23664 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   209672 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    59836 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:09:57.000000 tencentcloud-sdk-python-dnspod-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.912/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,17 @@
 
 # 您已经提交过申请并且正在审核中，请耐心等候。
 INVALIDPARAMETER_HASPENDINGAPPLY = 'InvalidParameter.HasPendingApply'
 
 # 该订单存在冲突或参数有误，无法完成支付，请重新购买。
 INVALIDPARAMETER_ILLEGALNEWDEAL = 'InvalidParameter.IllegalNewDeal'
 
+# 任务不存在。
+INVALIDPARAMETER_INNERTASKNOTEXIST = 'InvalidParameter.InnerTaskNotExist'
+
 # 礼券代码无效。
 INVALIDPARAMETER_INVALIDCOUPON = 'InvalidParameter.InvalidCoupon'
 
 # 请输入正确的订单号。
 INVALIDPARAMETER_INVALIDDEALNAME = 'InvalidParameter.InvalidDealName'
 
 # 无效密钥 ID。
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/v20210323/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.913/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.912/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.913/setup.py`

 * *Files identical despite different names*

