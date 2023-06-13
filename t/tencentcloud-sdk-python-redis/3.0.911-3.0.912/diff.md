# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.911.tar", last modified: Fri Jun  9 02:25:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.912.tar", last modified: Mon Jun 12 03:09:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.911.tar` & `tencentcloud-sdk-python-redis-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    87184 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297548 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:25:01.000000 tencentcloud-sdk-python-redis-3.0.911/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-12 03:09:47.000000 tencentcloud-sdk-python-redis-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    87184 2023-06-12 03:09:47.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-06-12 03:09:47.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:09:47.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297548 2023-06-12 03:09:47.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:09:47.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:09:47.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-12 03:09:47.000000 tencentcloud-sdk-python-redis-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:09:48.000000 tencentcloud-sdk-python-redis-3.0.912/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.911/README.rst` & `tencentcloud-sdk-python-redis-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/v20180412/redis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.911/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.912/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7130,15 +7130,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param NodeType: 节点类型。<ul><li>0：为主节点。</li><li>1：为副本节点。</li></ul>
         :type NodeType: int
-        :param NodeId: 主节点或者副本节点的 ID。<ul><li>该参数用于创建 Redis 实例接口[CreateInstances](https://cloud.tencent.com/document/product/239/20026) 并不需要设置，而用于变更实例配置的接口 [UpgradeInstance]删除副本(https://cloud.tencent.com/document/product/239/20013) 时才需要设置。</li><li>该参数可使用接口 [DescribeInstances](https://cloud.tencent.com/document/product/239/20018) 获取Integer类型的节点 ID。</li></ul>
+        :param NodeId: 主节点或者副本节点的 ID。<ul><li>该参数用于创建 Redis 实例接口[CreateInstances](https://cloud.tencent.com/document/product/239/20026) 并不需要设置，而用于变更实例配置的接口 [UpgradeInstance](https://cloud.tencent.com/document/product/239/20013) 删除副本时才需要设置。</li><li>该参数可使用接口 [DescribeInstances](https://cloud.tencent.com/document/product/239/20018) 获取Integer类型的节点 ID。</li></ul>
         :type NodeId: int
         :param ZoneId: 主节点或者副本节点的可用区 ID。
         :type ZoneId: int
         :param ZoneName: 主节点或者副本节点的可用区名称。
         :type ZoneName: str
         """
         self.NodeType = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.911/setup.py` & `tencentcloud-sdk-python-redis-3.0.912/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.911/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.912/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

