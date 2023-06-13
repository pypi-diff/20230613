# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.912.tar", last modified: Mon Jun 12 03:00:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.913.tar", last modified: Tue Jun 13 02:08:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.912.tar` & `tencentcloud-sdk-python-cvm-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119300 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)    43461 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   430455 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:00:59.000000 tencentcloud-sdk-python-cvm-3.0.912/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119300 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    43660 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   430455 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:08:50.000000 tencentcloud-sdk-python-cvm-3.0.913/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.912/README.rst` & `tencentcloud-sdk-python-cvm-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,14 +340,17 @@
 
 # 重复标签。
 INVALIDPARAMETERVALUE_DUPLICATETAGS = 'InvalidParameterValue.DuplicateTags'
 
 # 非GPU实例不允许转为GPU实例。
 INVALIDPARAMETERVALUE_GPUINSTANCEFAMILY = 'InvalidParameterValue.GPUInstanceFamily'
 
+# 您的高性能计算集群已经绑定其他可用区，不能购买当前可用区机器。
+INVALIDPARAMETERVALUE_HPCCLUSTERIDZONEIDNOTMATCH = 'InvalidParameterValue.HpcClusterIdZoneIdNotMatch'
+
 # IP格式非法。
 INVALIDPARAMETERVALUE_IPADDRESSMALFORMED = 'InvalidParameterValue.IPAddressMalformed'
 
 # ipv6地址无效
 INVALIDPARAMETERVALUE_IPV6ADDRESSMALFORMED = 'InvalidParameterValue.IPv6AddressMalformed'
 
 # HostName参数值不合法
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/cvm/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.913/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.912/setup.py` & `tencentcloud-sdk-python-cvm-3.0.913/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.912/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.913/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

