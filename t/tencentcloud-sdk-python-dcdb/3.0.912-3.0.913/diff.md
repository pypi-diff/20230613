# Comparing `tmp/tencentcloud-sdk-python-dcdb-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-dcdb-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.912.tar", last modified: Mon Jun 12 03:02:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.913.tar", last modified: Tue Jun 13 02:09:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dcdb-3.0.912.tar` & `tencentcloud-sdk-python-dcdb-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud_sdk_python_dcdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/v20180411/
--rw-r--r--   0 root         (0) root         (0)    13928 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/v20180411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/v20180411/__init__.py
--rw-r--r--   0 root         (0) root         (0)   243265 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/v20180411/models.py
--rw-r--r--   0 root         (0) root         (0)    71121 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/v20180411/dcdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:02:00.000000 tencentcloud-sdk-python-dcdb-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud_sdk_python_dcdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 02:09:46.000000 tencentcloud-sdk-python-dcdb-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/v20180411/
+-rw-r--r--   0 root         (0) root         (0)    13928 2023-06-13 02:09:46.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/v20180411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:46.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/v20180411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   243530 2023-06-13 02:09:46.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/v20180411/models.py
+-rw-r--r--   0 root         (0) root         (0)    71121 2023-06-13 02:09:46.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/v20180411/dcdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:46.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:09:46.000000 tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-13 02:09:46.000000 tencentcloud-sdk-python-dcdb-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.912/README.rst` & `tencentcloud-sdk-python-dcdb-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/v20180411/errorcodes.py` & `tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/v20180411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/v20180411/models.py` & `tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/v20180411/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2691,14 +2691,16 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExclusterType: int
         :param RsAccessStrategy: VPC就近访问
 注意：此字段可能返回 null，表示取不到有效值。
         :type RsAccessStrategy: int
         :param ReservedNetResources: 尚未回收的网络资源
         :type ReservedNetResources: list of ReservedNetResource
+        :param IsPhysicalReplicationSupported: 是否支持物理复制
+        :type IsPhysicalReplicationSupported: bool
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.InstanceId = None
         self.InstanceName = None
         self.Status = None
         self.StatusDesc = None
@@ -2745,14 +2747,15 @@
         self.InstanceType = None
         self.IsMaxUserConnectionsSupported = None
         self.DbVersionId = None
         self.EncryptStatus = None
         self.ExclusterType = None
         self.RsAccessStrategy = None
         self.ReservedNetResources = None
+        self.IsPhysicalReplicationSupported = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.Status = params.get("Status")
@@ -2815,14 +2818,15 @@
         self.RsAccessStrategy = params.get("RsAccessStrategy")
         if params.get("ReservedNetResources") is not None:
             self.ReservedNetResources = []
             for item in params.get("ReservedNetResources"):
                 obj = ReservedNetResource()
                 obj._deserialize(item)
                 self.ReservedNetResources.append(obj)
+        self.IsPhysicalReplicationSupported = params.get("IsPhysicalReplicationSupported")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeDCDBInstanceNodeInfoRequest(AbstractModel):
     """DescribeDCDBInstanceNodeInfo请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/dcdb/v20180411/dcdb_client.py` & `tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/dcdb/v20180411/dcdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dcdb-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dcdb-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.913/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.912/setup.py` & `tencentcloud-sdk-python-dcdb-3.0.913/setup.py`

 * *Files identical despite different names*

