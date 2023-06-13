# Comparing `tmp/clife_svc-1.12.tar.gz` & `tmp/clife_svc-1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clife_svc-1.12.tar", last modified: Tue May 16 02:54:47 2023, max compression
+gzip compressed data, was "dist\clife_svc-1.13.tar", last modified: Tue Jun 13 07:22:14 2023, max compression
```

## Comparing `clife_svc-1.12.tar` & `clife_svc-1.13.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.636510 clife_svc-1.12/
--rw-rw-rw-   0        0        0      420 2023-05-16 02:54:47.635459 clife_svc-1.12/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.12/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.555934 clife_svc-1.12/clife_svc/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.12/clife_svc/__init__.py
--rw-rw-rw-   0        0        0    12238 2023-04-27 10:53:11.000000 clife_svc-1.12/clife_svc/application.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.580068 clife_svc-1.12/clife_svc/config/
--rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.12/clife_svc/config/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.12/clife_svc/config/configmap.py
--rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.12/clife_svc/config/disconf.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.596253 clife_svc-1.12/clife_svc/errors/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.12/clife_svc/errors/__init__.py
--rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.12/clife_svc/errors/error_code.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.634456 clife_svc-1.12/clife_svc/libs/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.12/clife_svc/libs/__init__.py
--rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.12/clife_svc/libs/context.py
--rw-rw-rw-   0        0        0    14511 2023-05-15 11:07:39.000000 clife_svc-1.12/clife_svc/libs/http_request.py
--rw-rw-rw-   0        0        0     2649 2023-05-15 11:06:18.000000 clife_svc-1.12/clife_svc/libs/log.py
--rw-rw-rw-   0        0        0     3461 2023-01-13 06:23:00.000000 clife_svc-1.12/clife_svc/libs/mq_handler.py
--rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.12/clife_svc/libs/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.564962 clife_svc-1.12/clife_svc.egg-info/
--rw-rw-rw-   0        0        0      420 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 02:54:47.636510 clife_svc-1.12/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-05-16 02:54:25.000000 clife_svc-1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/
+drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc/
+-rw-rw-rw-   0        0        0    11780 2023-06-13 07:15:59.000000 clife_svc-1.13/clife_svc/application.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc/config/
+-rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.13/clife_svc/config/configmap.py
+-rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.13/clife_svc/config/disconf.py
+-rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.13/clife_svc/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc/errors/
+-rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.13/clife_svc/errors/error_code.py
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.13/clife_svc/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc/libs/
+-rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.13/clife_svc/libs/context.py
+-rw-rw-rw-   0        0        0    14499 2023-06-13 07:17:16.000000 clife_svc-1.13/clife_svc/libs/http_request.py
+-rw-rw-rw-   0        0        0     2649 2023-05-15 11:06:18.000000 clife_svc-1.13/clife_svc/libs/log.py
+-rw-rw-rw-   0        0        0     3510 2023-06-13 07:17:16.000000 clife_svc-1.13/clife_svc/libs/mq_handler.py
+-rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.13/clife_svc/libs/utils.py
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.13/clife_svc/libs/__init__.py
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.13/clife_svc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      420 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      535 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 07:22:14.000000 clife_svc-1.13/clife_svc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      420 2023-06-13 07:22:14.000000 clife_svc-1.13/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.13/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:22:14.000000 clife_svc-1.13/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-13 07:19:32.000000 clife_svc-1.13/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `clife_svc-1.12/clife_svc/application.py` & `clife_svc-1.13/clife_svc/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,15 @@
 
 """
 import os
 import re
 import time
 import threading
 import json
-from typing import (
-    Any,
-    Callable,
-    List,
-    Optional,
-    Set,
-    Union,
-)
+from typing import Any, Callable, List, Optional, Set, Union
 
 from fastapi import FastAPI, APIRouter, Request, Response
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import ORJSONResponse
 from fastapi.routing import APIRoute
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request as HttpRequest
@@ -34,41 +27,35 @@
 from clife_svc.errors.error_code import ApiException
 from clife_svc.libs.http_request import ClientRequest
 from clife_svc.libs.log import init_log, klogger, tlogger
 from clife_svc.libs.mq_handler import MQHandler
 
 
 class AiServiceRoute(APIRoute):
-
     def get_route_handler(self) -> Callable:
         original_route_handler = super().get_route_handler()
-
         async def custom_route_handler(request: Request) -> Response:
             body = await request.body()
             if request.query_params:
                 klogger.info('Request Params: {}'.format(request.query_params))
             if body:
                 try:
                     klogger.info('Request Body: {}'.format(json.loads(body.decode('utf-8'))))
                 except:
                     klogger.info('Request Body: {}'.format(body.decode('utf-8')))
             before = time.time()
-            # 这里可以获取的我们的请求体的信息----
             response: Response = await original_route_handler(request)
-
-            # 下面可以处理我们的响应体的报文信息，未被异常处理器拦截的请求将继续执行
             duration = time.time() - before
             if request.scope['path'] == '/time':
                 tlogger.info('Request Cost: {}s'.format(round(duration, 2)))
                 tlogger.info('Response Content: {}'.format(response.body.decode('utf-8')))
             else:
                 klogger.info('Request Cost: {}s'.format(round(duration, 2)))
                 klogger.info('Response Content: {}'.format(response.body.decode('utf-8')))
             return response
-
         return custom_route_handler
 
 
 class App(object):
     """
     http接口服务上下文对象，单实例对象
     """
@@ -95,22 +82,22 @@
         """
 
         # app_name参数校验
 
         if not re.match(r'^([a-zA-Z0-9]+-?[a-zA-Z0-9]+)+$', app_name):
             raise Exception('app_name can only be letters, numbers, or strike-through!')
 
-        self.__app_name = app_name
+        self.app_name = app_name
         init_log(os.path.join(log_root_path, app_name), log_level=log_level)
 
         self.__disconf_item = Disconf('clife-ai', '0.0.1-SNAPSHOT', conf).get_disconf()
         self.__configmap = ConfigMap()
 
         self.__ClientRequest = ClientRequest(self)
-        self.__MQHandler = MQHandler(app=self, app_name=app_name)
+        self.__MQHandler = MQHandler(app=self)
 
         self.__fast_api = FastAPI(title='ai-service', default_response_class=ORJSONResponse)
         self.__ai_router = APIRouter(route_class=AiServiceRoute)
 
     def init_api(self) -> FastAPI:
         """
         在App中初始化服务接口
@@ -129,20 +116,14 @@
                                        allow_credentials=True,
                                        allow_origins=["*"],
                                        allow_methods=["*"],
                                        allow_headers=["*"], )
         self.__fast_api.add_middleware(Interceptor)
 
     def get_conf(self, key: str, default: str = '') -> str:
-        """
-        获取disconf或ConfigMap挂载文件或环境变量的配置信息
-        :param key:配置项的key
-        :param default:配置项默认值
-        :return:
-        """
         if key in self.__disconf_item:
             return self.__disconf_item.get(key)
         item = self.__configmap.get(key)
         if item:
             return item
         item = utils.get_env(key)
         if item:
@@ -212,24 +193,24 @@
 
     async def upload_file(self, file_path: str, retry=2) -> str:
         """
         :param file_path:本地文件路径
         :param retry:失败重试次数，默认为2次，建议不大于3次
         :return: 文件url
         """
-        return await self.__ClientRequest.upload_file(self.__app_name, file_path, retry)
+        return await self.__ClientRequest.upload_file(self.app_name, file_path, retry)
 
     async def upload_file_from_buffer(self, file_extension: str, body, retry=2) -> str:
         """
         :param file_extension: 文件扩展名，如.txt|.png
         :param body: 文件流,必须实现了read方法
         :param retry: 失败重试次数,默认为2次，建议不大于3次
         :return: 文件url
         """
-        return await self.__ClientRequest.upload_file_from_buffer(self.__app_name, file_extension, body, retry)
+        return await self.__ClientRequest.upload_file_from_buffer(self.app_name, file_extension, body, retry)
 
     async def send_mq_msg(self, body, topic=None, keys=None, tags=None):
         """
         :param body: rocketMQ消息内容
         :param topic: rocketMQ消息主题，非必传，未配置默认主题时必传
         :param keys: rocketMQ消息唯一标识，非必传
         :param tags: rocketMQ消息标签，非必传
```

### Comparing `clife_svc-1.12/clife_svc/config/configmap.py` & `clife_svc-1.13/clife_svc/config/configmap.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.12/clife_svc/config/disconf.py` & `clife_svc-1.13/clife_svc/config/disconf.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.12/clife_svc/errors/error_code.py` & `clife_svc-1.13/clife_svc/errors/error_code.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.12/clife_svc/libs/http_request.py` & `clife_svc-1.13/clife_svc/libs/http_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,23 +155,22 @@
                 try:
                     resp_byte = await self._async_request('GET', file_url, resp_type='byte', timeout=timeout)
                     if not resp_byte:
                         raise DownloadFileException(data='Download file failed, url:{}'.format(file_url))
                     klogger.info('Download file cost: {}s'.format(round(time.time() - start, 2)))
                     klogger.info('Success download file.')
                     return resp_byte
-                # 捕获超时类型异常进行重试
-                except (ServerTimeoutError, asyncio.TimeoutError):
+                except Exception as e:
                     if retry != 0:
                         klogger.warning('Error download file,retry left: {}'.format(retry))
                         retry -= 1
                         continue
-                    raise TimeoutException(data='Download file timeout, url:{}'.format(file_url))
-                # 非超时异常直接抛出
-                except:
+                    # 超时类型异常
+                    if isinstance(e, ServerTimeoutError) or isinstance(e, asyncio.TimeoutError):
+                        raise TimeoutException(data='Download file timeout, url:{}'.format(file_url))
                     raise DownloadFileException(data='Download file failed, url:{}'.format(file_url))
         else:
             # 本地文件路径格式直接返回
             klogger.info('File path: {}'.format(file_url))
             return ''
 
     @staticmethod
```

### Comparing `clife_svc-1.12/clife_svc/libs/log.py` & `clife_svc-1.13/clife_svc/libs/log.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.12/clife_svc/libs/mq_handler.py` & `clife_svc-1.13/clife_svc/libs/mq_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 from clife_svc.libs.log import klogger, clogger
 
 
 class MQHandler:
 
-    def __init__(self, app, app_name):
+    def __init__(self, app):
         self._app = app
         self._producer = None
         self._producer_topic = None
         self._consumer = None
         self._consumer_group = None
         self._consumer_sub_topics = []
         try:
             from rocketmq.client import Producer, PushConsumer, Message
         except NotImplementedError:
             clogger.warning(f'rocketMQ does not support Windows, Message Queue disabled.')
         else:
             try:
-                rocket_url = app.get_conf('rocket.mq.url')
-                if rocket_url:
-                    clogger.info(f'rocketMQ URL: {rocket_url}')
-                    # 创建生产者
-                    self._producer = Producer(app_name)
-                    self._producer.set_namesrv_addr(rocket_url)
-                    self._producer.start()
+                self._rocket_url = app.get_conf('rocket.mq.url')
+                if self._rocket_url:
+                    clogger.info(f'rocketMQ URL: {self._rocket_url}')
                     self._producer_topic = app.get_conf('rocket.mq.producer.topic')
                     if not self._producer_topic:
                         clogger.warning(f'rocketMQ Producer: Default topic not found. Topic required when send message.')
                     # 创建消费者
                     self._consumer_group = app.get_conf('rocket.mq.consumer.group')
                     if not self._consumer_group:
                         clogger.warning(f'rocketMQ Consumer: consumer group not found, consumer disabled.')
                     else:
                         self._consumer = PushConsumer(self._consumer_group)
-                        self._consumer.set_namesrv_addr(rocket_url)
+                        self._consumer.set_namesrv_addr(self._rocket_url)
                 else:
                     clogger.warning(f'rocketMQ URL not found, Message Queue disabled.')
             except Exception as e:
                 clogger.warning(f'Error connect rocketMQ, Message Queue disabled.error_info:{e}')
 
     def add_subscribe(self, call_back, topic=None):
         if self._consumer:
@@ -54,23 +50,29 @@
             raise Exception('rocketMQ consumer disabled')
 
     def start_consumer(self):
         if len(self._consumer_sub_topics) > 0:
             self._consumer.start()
 
     def send_sync(self, body, topic=None, keys=None, tags=None):
-        from rocketmq.client import Message
-        if self._producer:
-            topic = topic if topic else self._producer_topic
-            if topic:
-                msg = Message(topic)  # noqa
-                msg.set_body(body)
-                if keys:
-                    msg.set_keys(keys)
-                if tags:
-                    msg.set_tags(tags)
-                self._producer.send_sync(msg)
-                klogger.info('rocketMQ message send success')
+        if not self._producer:
+            from rocketmq.client import Producer
+            if self._rocket_url:
+                self._producer = Producer(self._app.app_name)
+                self._producer.set_namesrv_addr(self._rocket_url)
+                self._producer.start()
             else:
-                raise Exception('Topic is required for rocketMQ producer')
+                raise Exception('rocketMQ URL not found, Message Queue disabled.')
+
+        topic = topic if topic else self._producer_topic
+        if topic:
+            from rocketmq.client import Message
+            msg = Message(topic)
+            msg.set_body(body)
+            if keys:
+                msg.set_keys(keys)
+            if tags:
+                msg.set_tags(tags)
+            self._producer.send_sync(msg)
+            klogger.info('rocketMQ message sent successfully')
         else:
-            raise Exception('rocketMQ producer disabled')
+            raise Exception('Topic is required for rocketMQ producer')
```

### Comparing `clife_svc-1.12/clife_svc/libs/utils.py` & `clife_svc-1.13/clife_svc/libs/utils.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.12/clife_svc.egg-info/SOURCES.txt` & `clife_svc-1.13/clife_svc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clife_svc-1.12/setup.py` & `clife_svc-1.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if line.startswith('-e git+'):
             dependency_links.append(line.replace('-e ', ''))
         else:
             requirements.append(line)
 
 setuptools.setup(
     name='clife_svc',   # 需要打包的名字,即本模块要发布的名字
-    version='1.12',     # 版本
+    version='1.13',     # 版本
     author='andy.hu',  # 作者名
     author_email='hlp0@163.com',  # 作者邮件
     description='A module for service',   # 简要描述
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',       # 项目地址,一般是代码托管的网站
     packages=setuptools.find_packages(),
```

