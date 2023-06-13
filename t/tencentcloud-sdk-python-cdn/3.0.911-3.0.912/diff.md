# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.911.tar", last modified: Fri Jun  9 02:14:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.912.tar", last modified: Mon Jun 12 02:58:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.911.tar` & `tencentcloud-sdk-python-cdn-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21972 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   573526 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   573678 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 02:58:47.000000 tencentcloud-sdk-python-cdn-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.911/README.rst` & `tencentcloud-sdk-python-cdn-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.912/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10917,18 +10917,19 @@
     + 热备源站回源域名配置
 
     """
 
     def __init__(self):
         r"""
         :param Origins: 主源站列表
-修改源站时，需要同时填充对应的 OriginType
+<font color=red>修改源站时，需要同时填充对应的 OriginType</font>
 注意：此字段可能返回 null，表示取不到有效值。
         :type Origins: list of str
         :param OriginType: 主源站类型
+<font color=red>当源站列表 Origins 不为空时必填</font>
 入参支持以下几种类型：
 domain：域名类型
 domainv6：域名解析V6类型
 cos：对象存储源站
 third_party: 第三方存储源站
 igtm: IGTM多活源
 ip：IP 列表作为源站
@@ -10947,37 +10948,39 @@
 出参增加以下几种类型：
 image：数据万象源站
 ftp：历史 FTP 托管源源站，现已不维护
 修改 Origins 时需要同时填充对应的 OriginType
 IPv6 功能目前尚未全量，需要先申请试用
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginType: str
-        :param ServerName: 当源站类型为cos或者第三方存储加速时,ServerName字段必填
-回主源站时 Host 头部，不填充则默认为加速域名
+        :param ServerName: 回主源站时 Host 头部
+<font color=red>当源站类型为cos或者第三方存储加速时,ServerName字段必填</font>
+不填充则默认为加速域名
 若接入的是泛域名，则回源 Host 默认为访问时的子域名
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServerName: str
         :param CosPrivateAccess: OriginType 为对象存储（COS）时，可以指定是否允许访问私有 bucket
 注意：需要先授权 CDN 访问该私有 Bucket 的权限后，才可开启此配置。取值范围: on/off
 注意：此字段可能返回 null，表示取不到有效值。
         :type CosPrivateAccess: str
         :param OriginPullProtocol: 回源协议配置
 http：强制 http 回源
 follow：协议跟随回源
 https：强制 https 回源，https 回源时仅支持源站 443 端口
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginPullProtocol: str
         :param BackupOrigins: 备源站列表
-修改备源站时，需要同时填充对应的 BackupOriginType
+<font color=red>修改备源站时，需要同时填充对应的 BackupOriginType</font>
 注意：此字段可能返回 null，表示取不到有效值。
         :type BackupOrigins: list of str
-        :param BackupOriginType: 备源站类型，支持以下类型：
+        :param BackupOriginType: 备源站类型
+<font color=red>备源站列表BackupOrigins 不为空时必填</font>
+支持以下类型：
 domain：域名类型
 ip：IP 列表作为源站
-修改 BackupOrigins 时需要同时填充对应的 BackupOriginType
 以下备源源站类型尚未全量支持，需要申请试用：
 ipv6_domain: 源站列表为多个 IPv6 地址以及域名
 ip_ipv6：源站列表为多个 IPv4 地址和IPv6 地址
 ipv6_domain: 源站列表为多个 IPv6 地址以及域名
 ip_ipv6_domain：源站列表为多个 IPv4 地址IPv6 地址以及域名
 注意：此字段可能返回 null，表示取不到有效值。
         :type BackupOriginType: str
@@ -10995,15 +10998,17 @@
         :type PathBasedOrigin: list of PathBasedOriginRule
         :param Sni: HTTPS回源SNI配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type Sni: :class:`tencentcloud.cdn.v20180606.models.OriginSni`
         :param AdvanceHttps: HTTPS回源高级配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type AdvanceHttps: :class:`tencentcloud.cdn.v20180606.models.AdvanceHttps`
-        :param OriginCompany: 对象存储回源厂商，当源站类型为第三方存储源站(third_party)时必填，可选值包括以下:
+        :param OriginCompany: 对象存储回源厂商
+<font color=red>当源站类型为第三方存储源站(third_party)时必填</font>
+可选值包括以下:
 aws_s3: AWS S3
 ali_oss: 阿里云 OSS
 hw_obs: 华为 OBS
 qiniu_kodo: 七牛云 kodo
 others: 其它厂商对象存储,仅支持兼容以AWS签名算法的对象存储，如腾讯云金融专区COS
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginCompany: str
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.912/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.911/setup.py` & `tencentcloud-sdk-python-cdn-3.0.912/setup.py`

 * *Files identical despite different names*

