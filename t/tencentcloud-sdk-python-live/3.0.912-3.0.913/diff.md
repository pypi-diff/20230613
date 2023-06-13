# Comparing `tmp/tencentcloud-sdk-python-live-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.912.tar", last modified: Mon Jun 12 03:06:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.913.tar", last modified: Tue Jun 13 02:14:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.912.tar` & `tencentcloud-sdk-python-live-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137299 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18702 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   433941 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:06:57.000000 tencentcloud-sdk-python-live-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137300 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18702 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   433875 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:14:23.000000 tencentcloud-sdk-python-live-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.912/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.913/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.912/README.rst` & `tencentcloud-sdk-python-live-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/live_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateLivePullStreamTask(self, request):
         """创建直播拉流任务。支持将外部已有的点播文件，或者直播源拉取过来转推到指定的目标地址。
         注意：
-        1. 默认支持任务数上限20个，如有特殊需求，可通过提单到售后进行评估增加上限。
+        1. 默认支持任务数上限200个，如有特殊需求，可通过提单到售后进行评估增加上限。
         2. 源流视频编码目前只支持: H264, H265。其他编码格式建议先进行转码处理。
         3. 源流音频编码目前只支持: AAC。其他编码格式建议先进行转码处理。
         4. 可在控制台开启过期自动清理，避免过期任务占用任务数额度。
         5. 拉流转推功能为计费增值服务，计费规则详情可参见[计费文档](https://cloud.tencent.com/document/product/267/53308)。
         6. 拉流转推功能仅提供内容拉取与推送服务，请确保内容已获得授权并符合内容传播相关的法律法规。若内容有侵权或违规相关问题，云直播会停止相关的功能服务并保留追究法律责任的权利。
 
         :param request: Request instance for CreateLivePullStreamTask.
```

### Comparing `tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.912/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.913/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1355,23 +1355,23 @@
         :type AppName: str
         :param StreamName: 推流名称。
 将拉取过来的流推到该流名称。
         :type StreamName: str
         :param StartTime: 开始时间。
 使用 UTC 格式时间，
 例如：2019-01-08T10:00:00Z。
-注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
+注意：北京时间值为 UTC 时间值 + 8 小时。
         :type StartTime: str
         :param EndTime: 结束时间，注意：
 1. 结束时间必须大于开始时间；
 2. 结束时间和开始时间必须大于当前时间；
 3. 结束时间 和 开始时间 间隔必须小于七天。
 使用 UTC 格式时间，
 例如：2019-01-08T10:00:00Z。
-注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
+注意：北京时间值为 UTC 时间值 + 8 小时。
         :type EndTime: str
         :param Operator: 任务操作人备注。
         :type Operator: str
         :param PushArgs: 推流参数。
 推流时携带自定义参数。
 示例：
 bak=1&test=2 。
@@ -1433,14 +1433,16 @@
 3. 支持的水印图片格式：png，jpg，gif 等。
         :type WatermarkList: list of PullPushWatermarkInfo
         :param VodLocalMode: 点播源是否启用本地推流模式，默认0，不启用。
 0 - 不启用。
 1 - 启用。
 注意：启用本地模式后，会将源列表中的 MP4 文件进行本地下载，优先使用本地已下载文件进行推流，提高点播源推流稳定性。使用本地下载文件推流时，会产生增值费用。
         :type VodLocalMode: int
+        :param RecordTemplateId: 录制模板 ID。
+        :type RecordTemplateId: str
         """
         self.SourceType = None
         self.SourceUrls = None
         self.DomainName = None
         self.AppName = None
         self.StreamName = None
         self.StartTime = None
@@ -1454,14 +1456,15 @@
         self.ExtraCmd = None
         self.Comment = None
         self.ToUrl = None
         self.BackupSourceType = None
         self.BackupSourceUrl = None
         self.WatermarkList = None
         self.VodLocalMode = None
+        self.RecordTemplateId = None
 
 
     def _deserialize(self, params):
         self.SourceType = params.get("SourceType")
         self.SourceUrls = params.get("SourceUrls")
         self.DomainName = params.get("DomainName")
         self.AppName = params.get("AppName")
@@ -1482,14 +1485,15 @@
         if params.get("WatermarkList") is not None:
             self.WatermarkList = []
             for item in params.get("WatermarkList"):
                 obj = PullPushWatermarkInfo()
                 obj._deserialize(item)
                 self.WatermarkList.append(obj)
         self.VodLocalMode = params.get("VodLocalMode")
+        self.RecordTemplateId = params.get("RecordTemplateId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-live-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.913/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.912/setup.py` & `tencentcloud-sdk-python-live-3.0.913/setup.py`

 * *Files identical despite different names*

