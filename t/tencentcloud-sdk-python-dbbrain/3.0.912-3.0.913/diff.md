# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.912.tar", last modified: Mon Jun 12 03:01:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.913.tar", last modified: Tue Jun 13 02:09:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.912.tar` & `tencentcloud-sdk-python-dbbrain-3.0.913.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    48612 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185526 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114440 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    48612 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185526 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   114440 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -766,43 +766,43 @@
 
     """
 
     def __init__(self):
         r"""
         :param InstanceId: 实例ID。
         :type InstanceId: str
-        :param SessionToken: 通过VerifyUserAccount获取有效期为5分钟的会话token，使用后会自动延长token有效期至五分钟后。
-        :type SessionToken: str
         :param SqlType: SQL类型，取值包括SELECT, UPDATE, DELETE, INSERT, REPLACE。
         :type SqlType: str
         :param FilterKey: 关键字，用于筛选SQL语句，多个关键字用英文逗号分隔，逗号不能作为关键词，多个关键词之间的关系为“逻辑与”。
         :type FilterKey: str
         :param MaxConcurrency: 最大并发度，取值不能小于0，如果该值设为 0，则表示限制所有匹配的SQL执行。
         :type MaxConcurrency: int
         :param Duration: 限流时长，单位秒，支持-1和小于2147483647的正整数，-1表示永不过期。
         :type Duration: int
+        :param SessionToken: 通过VerifyUserAccount获取有效期为5分钟的会话token，使用后会自动延长token有效期至五分钟后。
+        :type SessionToken: str
         :param Product: 服务产品类型，支持值："mysql" - 云数据库 MySQL；"cynosdb" - 云数据库 TDSQL-C for MySQL，默认为"mysql"。
         :type Product: str
         """
         self.InstanceId = None
-        self.SessionToken = None
         self.SqlType = None
         self.FilterKey = None
         self.MaxConcurrency = None
         self.Duration = None
+        self.SessionToken = None
         self.Product = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
-        self.SessionToken = params.get("SessionToken")
         self.SqlType = params.get("SqlType")
         self.FilterKey = params.get("FilterKey")
         self.MaxConcurrency = params.get("MaxConcurrency")
         self.Duration = params.get("Duration")
+        self.SessionToken = params.get("SessionToken")
         self.Product = params.get("Product")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -990,31 +990,31 @@
 
     """
 
     def __init__(self):
         r"""
         :param InstanceId: 实例ID。
         :type InstanceId: str
-        :param SessionToken: 通过VerifyUserAccount获取有效期为5分钟的会话token，使用后会自动延长token有效期至五分钟后。
-        :type SessionToken: str
         :param FilterIds: 限流任务ID列表。
         :type FilterIds: list of int
+        :param SessionToken: 通过VerifyUserAccount获取有效期为5分钟的会话token，使用后会自动延长token有效期至五分钟后。
+        :type SessionToken: str
         :param Product: 服务产品类型，支持值："mysql" - 云数据库 MySQL；"cynosdb" - 云数据库 TDSQL-C for MySQL，默认为"mysql"。
         :type Product: str
         """
         self.InstanceId = None
-        self.SessionToken = None
         self.FilterIds = None
+        self.SessionToken = None
         self.Product = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
-        self.SessionToken = params.get("SessionToken")
         self.FilterIds = params.get("FilterIds")
+        self.SessionToken = params.get("SessionToken")
         self.Product = params.get("Product")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3960,35 +3960,35 @@
 
     """
 
     def __init__(self):
         r"""
         :param InstanceId: 实例ID。
         :type InstanceId: str
-        :param SessionToken: 通过VerifyUserAccount获取有效期为5分钟的会话token，使用后会自动延长token有效期至五分钟后。
-        :type SessionToken: str
         :param FilterIds: SQL限流任务ID列表。
         :type FilterIds: list of int
         :param Status: 限流任务状态，取值支持TERMINATED - 终止。
         :type Status: str
+        :param SessionToken: 通过VerifyUserAccount获取有效期为5分钟的会话token，使用后会自动延长token有效期至五分钟后。
+        :type SessionToken: str
         :param Product: 服务产品类型，支持值："mysql" - 云数据库 MySQL；"cynosdb" - 云数据库 TDSQL-C for MySQL，默认为"mysql"。
         :type Product: str
         """
         self.InstanceId = None
-        self.SessionToken = None
         self.FilterIds = None
         self.Status = None
+        self.SessionToken = None
         self.Product = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
-        self.SessionToken = params.get("SessionToken")
         self.FilterIds = params.get("FilterIds")
         self.Status = params.get("Status")
+        self.SessionToken = params.get("SessionToken")
         self.Product = params.get("Product")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.913/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.912/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.913/setup.py`

 * *Files identical despite different names*

