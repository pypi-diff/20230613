# Comparing `tmp/tencentcloud-sdk-python-thpc-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-thpc-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.912.tar", last modified: Mon Jun 12 03:13:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.913.tar", last modified: Tue Jun 13 02:26:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-thpc-3.0.912.tar` & `tencentcloud-sdk-python-thpc-3.0.913.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20220401/
--rw-r--r--   0 root         (0) root         (0)     4733 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20220401/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20220401/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97393 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20220401/models.py
--rw-r--r--   0 root         (0) root         (0)    16733 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20220401/thpc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20211109/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20211109/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20211109/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43727 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20211109/models.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20211109/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20230321/
--rw-r--r--   0 root         (0) root         (0)     4248 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20230321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20230321/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107666 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20230321/models.py
--rw-r--r--   0 root         (0) root         (0)    17699 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20230321/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud_sdk_python_thpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:13:47.000000 tencentcloud-sdk-python-thpc-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20220401/
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20220401/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20220401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97393 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20220401/models.py
+-rw-r--r--   0 root         (0) root         (0)    16733 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20220401/thpc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20211109/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20211109/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20211109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20211109/models.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20211109/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20230321/
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20230321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20230321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107666 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20230321/models.py
+-rw-r--r--   0 root         (0) root         (0)    17699 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20230321/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud_sdk_python_thpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:26:52.000000 tencentcloud-sdk-python-thpc-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/README.rst` & `tencentcloud-sdk-python-thpc-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20220401/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20220401/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20220401/models.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20220401/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20220401/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20220401/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20211109/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20211109/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20211109/models.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20211109/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20211109/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20230321/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20230321/errorcodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,14 +109,17 @@
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
 
 # 弹性伸缩类型不支持此操作。
 UNSUPPORTEDOPERATION_AUTOSCALINGTYPE = 'UnsupportedOperation.AutoScalingType'
 
+# 集群资源正在处理其他请求。
+UNSUPPORTEDOPERATION_CLUSTERACCEPTOTHERREQUEST = 'UnsupportedOperation.ClusterAcceptOtherRequest'
+
 # 该集群当前状态不支持该操作。
 UNSUPPORTEDOPERATION_CLUSTERSTATUSNOTSUPPORT = 'UnsupportedOperation.ClusterStatusNotSupport'
 
 # 类型节点不支持当前操作。
 UNSUPPORTEDOPERATION_INVALIDNODEROLE = 'UnsupportedOperation.InvalidNodeRole'
 
 # 节点状态不支持此操作。
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20230321/models.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20230321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/thpc/v20230321/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/thpc/v20230321/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.913/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.913/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.912/setup.py` & `tencentcloud-sdk-python-thpc-3.0.913/setup.py`

 * *Files identical despite different names*

