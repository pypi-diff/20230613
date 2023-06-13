# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.912.tar", last modified: Mon Jun 12 03:06:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.913.tar", last modified: Tue Jun 13 02:14:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.912.tar` & `tencentcloud-sdk-python-lighthouse-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-12 03:06:48.000000 tencentcloud-sdk-python-lighthouse-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:06:48.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:06:48.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    26133 2023-06-12 03:06:48.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    92541 2023-06-12 03:06:48.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:06:48.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240371 2023-06-12 03:06:48.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-12 03:06:48.000000 tencentcloud-sdk-python-lighthouse-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:06:49.000000 tencentcloud-sdk-python-lighthouse-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    26133 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92541 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240373 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:14:18.000000 tencentcloud-sdk-python-lighthouse-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6260,15 +6260,15 @@
     """
 
     def __init__(self):
         r"""
         :param InstanceIds: 实例 ID 列表。每次请求批量实例的上限为 100。
         :type InstanceIds: list of str
         :param Password: 实例登录密码。不同操作系统类型密码复杂度限制不一样，具体如下：
-`LINUX_UNIX` 实例密码必须 8-30 位，推荐使用 12 位以上密码，不能以“/”开头，至少包含以下字符中的三种不同字符，字符种类：<br><li>小写字母：[a-z]<br><li>大写字母：[A-Z]<br><li>数字：0-9<br><li>特殊字符： ()\`~!@#$%^&\*-+=\_|{}[]:;'<>,.?/</li>
+`LINUX_UNIX` 实例密码必须 8-30 位，推荐使用 12 位以上密码，不能以“/”开头，至少包含以下字符中的三种不同字符，字符种类：<br><li>小写字母：[a-z]<br><li>大写字母：[A-Z]<br><li>数字：0-9<br><li>特殊字符： ()\`\~!@#$%^&\*-+=\_|{}[]:;' <>,.?/</li>
 `WINDOWS` 实例密码必须 12-30 位，不能以“/”开头且不包括用户名，至少包含以下字符中的三种不同字符<br><li>小写字母：[a-z]<br><li>大写字母：[A-Z]<br><li>数字： 0-9<br><li>特殊字符：()\`~!@#$%^&\*-+=\_|{}[]:;' <>,.?/<br><li>如果实例即包含 `LINUX_UNIX` 实例又包含 `WINDOWS` 实例，则密码复杂度限制按照 `WINDOWS` 实例的限制。
         :type Password: str
         :param UserName: 待重置密码的实例操作系统用户名。不得超过 64 个字符。
         :type UserName: str
         """
         self.InstanceIds = None
         self.Password = None
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.913/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.913/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.912/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.913/setup.py`

 * *Files identical despite different names*

