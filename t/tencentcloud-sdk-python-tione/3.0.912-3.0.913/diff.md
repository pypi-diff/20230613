# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.912.tar", last modified: Mon Jun 12 03:14:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.913.tar", last modified: Tue Jun 13 02:27:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.912.tar` & `tencentcloud-sdk-python-tione-3.0.913.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    11488 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   336462 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:14:26.000000 tencentcloud-sdk-python-tione-3.0.912/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    12587 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   336462 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:27:26.000000 tencentcloud-sdk-python-tione-3.0.913/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.912/README.rst` & `tencentcloud-sdk-python-tione-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 
 # 数据集操作不支持。
 FAILEDOPERATION_DCUNSUPPORTEDOPERATION = 'FailedOperation.DCUnsupportedOperation'
 
 # 名称重复。
 FAILEDOPERATION_DUPLICATENAME = 'FailedOperation.DuplicateName'
 
+# 训练任务名称已存在，请更换名称
+FAILEDOPERATION_DUPLICATENAMETASKISCREATING = 'FailedOperation.DuplicateNameTaskIsCreating'
+
 # 数据库执行错误。
 FAILEDOPERATION_EXECDATABASEFAIL = 'FailedOperation.ExecDatabaseFail'
 
 # 标签操作失败。
 FAILEDOPERATION_EXECTAGFAIL = 'FailedOperation.ExecTagFail'
 
 # 余额不足冻结失败。
@@ -166,14 +169,23 @@
 
 # 数据解析失败。
 FAILEDOPERATION_UNMARSHALDATA = 'FailedOperation.UnmarshalData'
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
+# 绑定标签失败
+INTERNALERROR_BINDINGTAGSFAILED = 'InternalError.BindingTagsFailed'
+
+# 创建JOB失败
+INTERNALERROR_CREATEJOBINSTANCEFAILED = 'InternalError.CreateJobInstanceFailed'
+
+# 创建TCR镜像仓库长期访问凭证失败
+INTERNALERROR_CREATETCRINSTANCETOKENFAILED = 'InternalError.CreateTcrInstanceTokenFailed'
+
 # 冻结失败。
 INTERNALERROR_FREEZEBILLFAILED = 'InternalError.FreezeBillFailed'
 
 # 余额不足。
 INTERNALERROR_INSUFFICIENTBALANCE = 'InternalError.InsufficientBalance'
 
 # 没有权限。
@@ -196,14 +208,17 @@
 
 # 查询子网信息失败。
 INTERNALERROR_QUERYSUBNETINFOFAILED = 'InternalError.QuerySubnetInfoFailed'
 
 # 停止任务失败。
 INTERNALERROR_STOPJOBINSTANCEFAILED = 'InternalError.StopJobInstanceFailed'
 
+# 未提交状态禁止停止
+INTERNALERROR_UNSUBMITTEDSTATUSNOTALLOWSTOP = 'InternalError.UnSubmittedStatusNotAllowStop'
+
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 模型包不符合规范。
 INVALIDPARAMETER_MODELFILEINVALID = 'InvalidParameter.ModelFileInvalid'
 
 # 无效的接口。
@@ -256,26 +271,35 @@
 
 # 实例名称冲突，请更换名称后重试。
 INVALIDPARAMETERVALUE_DUPLICATENAME = 'InvalidParameterValue.DuplicateName'
 
 # 训练框架对应的版本不支持，请阅读文档查看TIONE目前支持的框架和版本。
 INVALIDPARAMETERVALUE_FRAMEWORKVERSIONNOTSUPPORT = 'InvalidParameterValue.FrameworkVersionNotSupport'
 
+# 获取CFS的挂载IP失败
+INVALIDPARAMETERVALUE_GETCFSMOUNTIPFAILED = 'InvalidParameterValue.GetCFSMountIPFailed'
+
 # 训练任务镜像不存在。
 INVALIDPARAMETERVALUE_IMAGENOTFOUND = 'InvalidParameterValue.ImageNotFound'
 
 # 无效的过滤器。
 INVALIDPARAMETERVALUE_INVALIDFILTER = 'InvalidParameterValue.InvalidFilter'
 
 # 参数值数量超过限制。
 INVALIDPARAMETERVALUE_LIMITEXCEEDED = 'InvalidParameterValue.LimitExceeded'
 
 # 操作不允许。
 INVALIDPARAMETERVALUE_NOTALLOW = 'InvalidParameterValue.NotAllow'
 
+# 分页查询limit超出限制
+INVALIDPARAMETERVALUE_PAGELIMITEXCEEDED = 'InvalidParameterValue.PageLimitExceeded'
+
+# RDMA配置不合法
+INVALIDPARAMETERVALUE_RDMACONFIGILLEGAL = 'InvalidParameterValue.RDMAConfigIllegal'
+
 # 资源配置不合法
 INVALIDPARAMETERVALUE_RESOURCECONFIGILLEGAL = 'InvalidParameterValue.ResourceConfigIllegal'
 
 # 裸金属类型资源组不支持配置输入数据
 INVALIDPARAMETERVALUE_UNSUPPORTEDDATACONFIG = 'InvalidParameterValue.UnsupportedDataConfig'
 
 # 超过配额限制。
@@ -286,23 +310,29 @@
 
 # 操作被拒绝。
 OPERATIONDENIED = 'OperationDenied'
 
 # 余额不足，创建/更新失败。
 OPERATIONDENIED_BALANCEINSUFFICIENT = 'OperationDenied.BalanceInsufficient'
 
+# 计费平台出错
+OPERATIONDENIED_BILLINGEXCEPTION = 'OperationDenied.BillingException'
+
 # 按量计费资源售罄。
 OPERATIONDENIED_BILLINGSTATUSRESOURCEINSUFFICIENT = 'OperationDenied.BillingStatusResourceInsufficient'
 
 # 觅影资源包余额不足，请先充值。
 OPERATIONDENIED_MIYINGBALANCEINSUFFICIENT = 'OperationDenied.MIYINGBalanceInsufficient'
 
 # 网段不合法。
 OPERATIONDENIED_NETWORKCIDRILLEGAL = 'OperationDenied.NetworkCidrIllegal'
 
+# 操作不允许
+OPERATIONDENIED_NOTALLOW = 'OperationDenied.NotAllow'
+
 # 预付费资源组余量不足。
 OPERATIONDENIED_RESOURCEGROUPINSUFFICIENT = 'OperationDenied.ResourceGroupInsufficient'
 
 # 白名单免费配额不足。
 OPERATIONDENIED_WHITELISTQUOTAEXCEED = 'OperationDenied.WhitelistQuotaExceed'
 
 # 资源被占用。
```

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20211111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.913/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.912/setup.py` & `tencentcloud-sdk-python-tione-3.0.913/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.912/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.913/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

