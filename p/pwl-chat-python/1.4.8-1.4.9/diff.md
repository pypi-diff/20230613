# Comparing `tmp/pwl-chat-python-1.4.8.tar.gz` & `tmp/pwl-chat-python-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.8.tar", last modified: Sun Jun 11 13:51:50 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.9.tar", last modified: Tue Jun 13 10:07:08 2023, max compression
```

## Comparing `pwl-chat-python-1.4.8.tar` & `pwl-chat-python-1.4.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/__api__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/chatroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/redpacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/chatroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/redpacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:07:08.716922 pwl-chat-python-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/__api__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/chatroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/redpacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/chatroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/redpacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.8/LICENSE` & `pwl-chat-python-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.8/PKG-INFO` & `pwl-chat-python-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.8
+Version: 1.4.9
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
   ![摸鱼派cn.png](https://b3logfile.com/file/2023/05/摸鱼派-cn-owZQT8f.png)
 
 # pwl-chat-python
 
 > 摸鱼派聊天室 python 命令行客户端
 
 基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室 python 客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
 
 ## 安装
 
-环境: Python3.10 以上
+环境: Python3.9 以上
 
 执行
 
 ```bash
 pip install pwl-chat-python
 ```
 
@@ -82,14 +82,15 @@
     - 发红包🧧
       - 拼手气红包
       - 普通红包
       - 专属红包
       - 心跳红包
       - 猜拳红包
       - 设置抢红包等待时间
+      - 抢猜拳红包最大限制
 
 ## 效果
 
 ![image.png](https://file.fishpi.cn/2023/06/image-d4da9bf7.png)
 ![redpacket](https://file.fishpi.cn/2023/06/image-d0ad7756.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.8/README.md` & `pwl-chat-python-1.4.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 > 摸鱼派聊天室 python 命令行客户端
 
 基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室 python 客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
 
 ## 安装
 
-环境: Python3.10 以上
+环境: Python3.9 以上
 
 执行
 
 ```bash
 pip install pwl-chat-python
 ```
 
@@ -63,14 +63,15 @@
     - 发红包🧧
       - 拼手气红包
       - 普通红包
       - 专属红包
       - 心跳红包
       - 猜拳红包
       - 设置抢红包等待时间
+      - 抢猜拳红包最大限制
 
 ## 效果
 
 ![image.png](https://file.fishpi.cn/2023/06/image-d4da9bf7.png)
 ![redpacket](https://file.fishpi.cn/2023/06/image-d0ad7756.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.8/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.9/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.8
+Version: 1.4.9
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
   ![摸鱼派cn.png](https://b3logfile.com/file/2023/05/摸鱼派-cn-owZQT8f.png)
 
 # pwl-chat-python
 
 > 摸鱼派聊天室 python 命令行客户端
 
 基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室 python 客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
 
 ## 安装
 
-环境: Python3.10 以上
+环境: Python3.9 以上
 
 执行
 
 ```bash
 pip install pwl-chat-python
 ```
 
@@ -82,14 +82,15 @@
     - 发红包🧧
       - 拼手气红包
       - 普通红包
       - 专属红包
       - 心跳红包
       - 猜拳红包
       - 设置抢红包等待时间
+      - 抢猜拳红包最大限制
 
 ## 效果
 
 ![image.png](https://file.fishpi.cn/2023/06/image-d4da9bf7.png)
 ![redpacket](https://file.fishpi.cn/2023/06/image-d0ad7756.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.8/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.9/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.8/setup.py` & `pwl-chat-python-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Package meta-data.
 NAME = 'pwl-chat-python'
 DESCRIPTION = '摸鱼派聊天室python客户端'
 URL = 'https://github.com/gakkiyomi/pwl-chat-python'
 EMAIL = 'gakkiyomi@gmail.com'
 AUTHOR = 'gakkiyomi'
-REQUIRES_PYTHON = '>=3.10.8'
+REQUIRES_PYTHON = '>=3.9'
 VERSION = __version__
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests', 'websocket-client', 'click', 'schedule'
 ]
```

### Comparing `pwl-chat-python-1.4.8/src/api/__init__.py` & `pwl-chat-python-1.4.9/src/api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,9 +46,18 @@
         elif rsp['code'] == -1 and rsp['msg'] == '两步验证失败，请填写正确的一次性密码':
             print("请输入两步验证码:")
             return False
         else:
             print(f"登陆失败: {rsp['msg']}")
             sys.exit(1)
 
+    def get_breezemoons(self, page:int = 1,size :int = 10) -> dict | None:
+        res = requests.get(f'{HOST}/api/breezemoons?p={page}&size={size}', headers={'User-Agent': UA})
+        print(res.text)
+        response = json.loads(res.text)
+        if 'code' in response and response['code'] == 0:
+            return response['breezemoons']
+        else:
+            print(response['msg'])
+            return None
 
 API = FishPi()
```

### Comparing `pwl-chat-python-1.4.8/src/api/chatroom.py` & `pwl-chat-python-1.4.9/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.8/src/api/redpacket.py` & `pwl-chat-python-1.4.9/src/api/redpacket.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,10 +37,8 @@
     def __init__(self, msg :str = '剪刀石头布!', money :int = 32, gesture :int = 0):
         super().__init__(msg, money, 1, RedPacketType.RPS)
         self.gesture = gesture
         
     def __json__(self):
         json_data = super().__json__()
         json_data['gesture'] = self.gesture
-        return json_data
-        
-        
+        return json_data
```

### Comparing `pwl-chat-python-1.4.8/src/api/user.py` & `pwl-chat-python-1.4.9/src/api/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,23 @@
          })
          response = json.loads(res.text)
          if 'code' in response and response['code'] == 0:
              print('清风明月发布成功')
          else:
              print(response['msg'])
 
+    def get_breezemoons(self, username :str, page:int = 1, size :int = 10) -> dict | None:
+        resp = requests.get(f'{HOST}/api/user/{username}/breezemoons?p={page}&size={size}&apiKey={self.api_key}', headers={'User-Agent': UA})
+        response = json.loads(resp.text)
+        if 'code' in response and response['code'] == 0:
+            return response['data']['breezemoons']
+        else:
+            print(response['msg'])
+            return None
+
     def checked_status(self) -> dict:
         resp = requests.get(f'{HOST}/user/checkedIn?apiKey={self.api_key}', headers={'User-Agent': UA})
         return json.loads(resp.text)
 
     def get_liveness_info(self) -> dict:
         resp = requests.get(f'{HOST}/user/liveness?apiKey={self.api_key}', headers={'User-Agent': UA})
         return json.loads(resp.text)
```

### Comparing `pwl-chat-python-1.4.8/src/core/__init__.py` & `pwl-chat-python-1.4.9/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.8/src/core/blacklist.py` & `pwl-chat-python-1.4.9/src/core/blacklist.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
-import os
 import re
 from src.api import FishPi
 from .config import GLOBAL_CONFIG
 
 
 def unban_someone(api: FishPi, username):
     if not GLOBAL_CONFIG.chat_config.blacklist.__contains__(username):
-        print(username + '不在小黑屋中')
+        print(f'{username}不在小黑屋中')
         return
     user_info = api.user.get_user_info(username)
     if user_info is None:
         return
     GLOBAL_CONFIG.chat_config.blacklist.remove(username)
     print(username + '已从小黑屋中释放')
     if GLOBAL_CONFIG.cfg_path is None:
@@ -28,21 +27,21 @@
             str(GLOBAL_CONFIG.chat_config.blacklist).replace("\'", "\"")
     dst.write(re.sub(r'blacklist.*', after, config_text))
     dst.close()
 
 
 def ban_someone(api: FishPi, username):
     if GLOBAL_CONFIG.chat_config.blacklist.__contains__(username):
-        print(username + ' 已在小黑屋中')
+        print(f'{username}已在小黑屋中')
         return
     user_info = api.user.get_user_info(username)
     if user_info is None:
         return
     GLOBAL_CONFIG.chat_config.blacklist.append(username)
-    print(username + '已加入到小黑屋中')
+    print(f'{username}已加入到小黑屋中')
     if GLOBAL_CONFIG.cfg_path is None:
         return
     # 持久化到文件
     src = open(GLOBAL_CONFIG.cfg_path, "r+")
     config_text = src.read()
     src.close()
     dst = open(GLOBAL_CONFIG.cfg_path, 'w')
```

### Comparing `pwl-chat-python-1.4.8/src/core/chatroom.py` & `pwl-chat-python-1.4.9/src/core/chatroom.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 import random
 import schedule
+from concurrent.futures import ThreadPoolExecutor
 from src.api import FishPi
 from .config import GLOBAL_CONFIG
 from .redpacket import rush_redpacket
 
 
 REPEAT_POOL = {}  # 复读池
 
@@ -25,33 +26,36 @@
 
 
 def soliloquize(api: FishPi) -> None:
     length = len(GLOBAL_CONFIG.chat_config.sentences)
     index = random.randint(0, length - 1)
     api.chatroom.send(GLOBAL_CONFIG.chat_config.sentences[index])
 
+executor = ThreadPoolExecutor(max_workers=5)
+
 def listener(api: FishPi, message :dict) -> None:
     if message['type'] == 'msg':
         if message['content'].find("redPacket") != -1:
-            rush_redpacket(api, message)
+            executor.submit(rush_redpacket, api, message)
+            #rush_redpacket(api, message)
         else:
             time = message['time']
             user = message['userName']
             user_nick_name = message['userNickname']
             if len(GLOBAL_CONFIG.chat_config.blacklist) > 0 \
                     and GLOBAL_CONFIG.chat_config.blacklist.__contains__(user):
                 return
             if user == GLOBAL_CONFIG.auth_config.username:
-                print('\t\t\t\t\t\t[' + time + ']')
-                print('\t\t\t\t\t\t你说: ' + message['md'])
+                print(f'\t\t\t\t\t\t[{time}]')
+                print(f'\t\t\t\t\t\t你说: {message["md"]}')
             else:
                 if 'client' in message:
-                    print('[' + time + '] 来自(' + message['client']+')')
+                    print(f'[{time}] 来自({message["client"]})')
                 else:
-                    print('[' + time + ']')
+                    print(f'[{time}]')
                 if len(user_nick_name) >0:
                     print(f'{user_nick_name}({user})说:')
                 else:
                     print(f'{user}说:')    
                 print(message['md'])
                 print('\r\n')
             if GLOBAL_CONFIG.chat_config.repeat_mode_switch:
```

### Comparing `pwl-chat-python-1.4.8/src/core/cli.py` & `pwl-chat-python-1.4.9/src/core/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,43 +8,51 @@
 
 
 
 def __send_redpacket_handler(api :FishPi, msg :str):
         if  msg == "#rp":
                api.chatroom.send_redpacket()
         elif msg == "#rp-ave":
-               api.chatroom.send_redpacket(RedPacket('人人有份!', 32, 5, RedPacketType.AVERAGE))
+               api.chatroom.send_redpacket(RedPacket('不要抢,人人有份!', 32, 5, RedPacketType.AVERAGE))
         elif msg == "#rp-hb":
-               api.chatroom.send_redpacket(RedPacket('慎点!', 32, 5, RedPacketType.HEARTBEAT))
+               api.chatroom.send_redpacket(RedPacket('玩的就是心跳!', 32, 5, RedPacketType.HEARTBEAT))
         elif msg == "#rp-rps":
                api.chatroom.send_redpacket(RPSRedPacket('剪刀石头布!', 32, 0))
         elif msg.startswith('#rp-to'):
             res = re.fullmatch(RP_SEND_TO_CODE_RE, msg)
             if res is not None:
-                api.chatroom.send_redpacket(SpecifyRedPacket('给你!', res.group(1), res.group(2).replace('，',',').split(",")))
+                api.chatroom.send_redpacket(SpecifyRedPacket('听我说谢谢你,因为有你,温暖了四季!', res.group(1), res.group(2).replace('，',',').split(",")))
             else:
                 print('非法红包指令')               
         elif msg.startswith('#rp-ave'):
             res = re.fullmatch(RP_AVER_CODE_RE,msg)
             if res is not None:
-                api.chatroom.send_redpacket(RedPacket('人人有份!', res.group(2), res.group(1), RedPacketType.AVERAGE))
+                api.chatroom.send_redpacket(RedPacket('不要抢,人人有份!', res.group(2), res.group(1), RedPacketType.AVERAGE))
             else:
                 print('非法红包指令')       
         elif msg.startswith('#rp-hb'):
             res = re.fullmatch(RP_HB_CODE_RE,msg)
             if res is not None:
-                api.chatroom.send_redpacket(RedPacket('人人有份!', res.group(2), res.group(1), RedPacketType.HEARTBEAT))
+                api.chatroom.send_redpacket(RedPacket('玩的就是心跳!', res.group(2), res.group(1), RedPacketType.HEARTBEAT))
             else:
                 print('非法红包指令')
         elif msg.startswith('#rp-rps'):
-            res = re.fullmatch(RP_RPS_CODE_RE,msg)
-            if res is not None:
-                api.chatroom.send_redpacket(RPSRedPacket('剪刀石头布!', res.group(2), res.group(1)))
-            else:
-                print('非法红包指令')
+            if msg.startswith('#rp-rps-limit'):
+                try:
+                    limit = msg.split(' ')[1]
+                    GLOBAL_CONFIG.redpacket_config.rps_limit = int(limit)
+                    print(f'猜拳红包限制设置{limit}成功')
+                except Exception:
+                    print('非法红包指令')
+            else:
+                res = re.fullmatch(RP_RPS_CODE_RE,msg)
+                if res is not None:
+                    api.chatroom.send_redpacket(RPSRedPacket('剪刀石头布!', res.group(2), res.group(1)))
+                else:
+                    print('非法红包指令')
         elif msg.startswith('#rp-time'):
             res = re.fullmatch(RP_TIME_CODE_RE,msg)
             if res is not None:
                 time = res.group(1)
                 GLOBAL_CONFIG.redpacket_config.rate = int(time)
                 print(f'红包等待时间已设置成功 {time}s')
             else:
@@ -76,14 +84,16 @@
             if api.ws == None:
                init_chatroom(api)
             else:
                chatroom_out(api)
                init_chatroom(api)
         elif msg.startswith('#bm'):
             api.user.send_breezemoon(msg[msg.find(' ')+1:len(msg)])
+        elif msg == '#api-key':
+            print(api.api_key)
         elif msg.startswith('#transfer'):
             res = re.fullmatch(TRANSFER_RE, msg)
             if res is not None:
                 api.user.transfer(res.group(2), res.group(1), res.group(3))
             else:
                print('非法转账命令')    
         elif msg.startswith('#rp'):
```

### Comparing `pwl-chat-python-1.4.8/src/core/config.py` & `pwl-chat-python-1.4.9/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.8/src/core/redpacket.py` & `pwl-chat-python-1.4.9/src/core/redpacket.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from src.api import FishPi
 import json
 import time
 import enum
-from src.utils import utils
+from src.utils.utils import RPS_LOSED, RPS_ZERO, RPS_SUCCESS
 from .config import GLOBAL_CONFIG
 
 CODE = enum.Enum('REDPACKET_CODE', ['SUCCESS', 'LOSED', 'NOT_ME', "ZERO"])
 
 
 def __open_redpacket_render(username, redpacket: dict) -> CODE:
     who = redpacket['who']
+    sender = redpacket['info']['userName']
     for i in who:
         if i['userName'] == username:
             if i['userMoney'] < 0:
-                print("红包助手: 悲剧，你竟然被反向抢了红包(" + str(i['userMoney']) + ")!")
+                print(f"红包助手: 悲剧，你竟然被{sender}反向抢了红包({str(i['userMoney'])})积分!")
                 return CODE.LOSED
             elif i['userMoney'] == 0:
-                print("红包助手: 零溢事件，抢到了一个空的红包(" + str(i['userMoney']) + ")!")
+                print(f"红包助手: 零溢事件，{sender}的红包抢到了({str(i['userMoney'])})积分!")
                 return CODE.ZERO
             else:
-                print("红包助手: 恭喜，你抢到了一个红包(" + str(i['userMoney']) + ")!")
+                print(f"红包助手: 恭喜，你抢到了{sender}的红包({str(i['userMoney'])})积分!")
                 return CODE.SUCCESS
-    print("红包助手: 遗憾，比别人慢了一点点，建议换宽带!")
+    print(f"红包助手: 遗憾 {sender}的红包没有抢到，比别人慢了一点点，建议换宽带!")
     return CODE.NOT_ME
 
 
 def open_red_packet(api: FishPi, red_packet_id) -> None:
     resp_json = api.chatroom.open_redpacket(red_packet_id)
     if ('code' in resp_json and resp_json['code'] == -1):
         print(resp_json['msg'])
@@ -36,54 +37,54 @@
 def open_rock_paper_scissors_packet(api: FishPi, red_packet_id) -> None:
     resp_json = api.chatroom.open_rock_paper_scissors_redpacket(red_packet_id)
     if ('code' in resp_json and resp_json['code'] == -1):
         print(resp_json['msg'])
         return
     code = __open_redpacket_render(api.current_user, resp_json)
     if code == CODE.SUCCESS:
-        api.chatroom.send(utils.RPS_SUCCESS)
+        api.chatroom.send(RPS_SUCCESS)
     elif code == CODE.LOSED:
-        api.chatroom.send(utils.RPS_LOSED)
+        api.chatroom.send(RPS_LOSED)
     elif code == CODE.ZERO:
-        api.chatroom.send(utils.RPS_ZERO)    
+        api.chatroom.send(RPS_ZERO)
 
 
 def rush_redpacket(api: FishPi, redpacket):
     sender = redpacket['userName']
     if sender == api.current_user:
         print('\t\t\t\t\t\t[' + redpacket['time'] + ']')
         print('\t\t\t\t\t\t发送了一个红包')
         return
     if (GLOBAL_CONFIG.redpacket_config.red_packet_switch == False):
-        print('红包助手: '+sender+'发送了一个红包 你错过了这个红包，请开启抢红包模式！')
+        print(f'红包助手: {sender}发送了一个红包 你错过了这个红包，请开启抢红包模式！')
         return
     sender = redpacket['userName']
     content = json.loads(redpacket['content'])
     if content['type'] == 'heartbeat':
         if GLOBAL_CONFIG.redpacket_config.heartbeat:
             if GLOBAL_CONFIG.redpacket_config.smart_mode:
-                print('红包助手: ' + sender + ' 发了一个心跳红包')
+                print(f'红包助手: {sender}发了一个心跳红包')
                 __analyzeHeartbeatRedPacket(api, redpacket['oId'])
                 return
             open_red_packet(api, redpacket['oId'])
         else:
-            print('红包助手: '+sender+' 发送了一个心跳红包, 你选择跳过了这个心跳红包！不尝试赌一下人品吗？')
+            print(f'红包助手: {sender}发送了一个心跳红包, 你选择跳过了这个心跳红包！不尝试赌一下人品吗？')
             return
     if content['type'] == 'rockPaperScissors':
         print(
             f'红包助手: {sender} 发送了一个猜拳红包, 但社区规定，助手抢红包要等{GLOBAL_CONFIG.redpacket_config.rate}秒哦～')
         time.sleep(GLOBAL_CONFIG.redpacket_config.rate)
         print('红包助手正在帮你猜拳，石头剪刀布！')
         money = content['money']
         if money > GLOBAL_CONFIG.redpacket_config.rps_limit:
             print(f'红包助手: {sender} 发送了一个积分为({money})的猜拳红包, 怂了 不敢赌～')
         else:
             open_rock_paper_scissors_packet(api, redpacket['oId'])
     else:
-        print('红包助手: ' + sender+' 发送了一个红包, 但社区规定，助手抢红包要等' +
+        print(f'红包助手: {sender} 发送了一个红包, 但社区规定，助手抢红包要等' +
               str(GLOBAL_CONFIG.redpacket_config.rate)+'秒哦～')
         time.sleep(GLOBAL_CONFIG.redpacket_config.rate)
         open_red_packet(api, redpacket['oId'])
 
 
 def __analyzeHeartbeatRedPacket(api: FishPi, red_packet_id):
     for data in api.chatroom.more()['data']:
@@ -96,23 +97,23 @@
     print("红包助手: 你与此红包无缘")
 
 
 def __analyze(api: FishPi, packet, red_packet_id, ctime, sender):
     count = packet['count']
     got = packet['got']
     if packet['count'] == packet['got']:
-        print('红包助手: '+sender+' 发送的心跳红包, 遗憾没有抢到，比别人慢了一点点，建议换宽带!')
+        print(f'红包助手: {sender} 发送的心跳红包, 遗憾没有抢到，比别人慢了一点点，建议换宽带!')
         return
 
     probability = 1 / (count - got)
     for get in packet['who']:
         if get['userMoney'] > 0:
             print('红包助手: '+sender+' 发送的心跳红包已无效，智能跳坑！')
             return
-    print('红包助手: 此心跳红包的中奖概率为:'+str(probability))
+    print(f'红包助手: 此心跳红包的中奖概率为:{str(probability)}')
     if probability >= GLOBAL_CONFIG.redpacket_config.threshold:
         open_red_packet(api, red_packet_id)
     else:
         timeArray = time.strptime(ctime, "%Y-%m-%d %H:%M:%S")
         timeStamp = int(time.mktime(timeArray))
         if int(time.time()) - timeStamp > GLOBAL_CONFIG.redpacket_config.timeout:
             if GLOBAL_CONFIG.redpacket_config.adventure_mode:
```

### Comparing `pwl-chat-python-1.4.8/src/core/user.py` & `pwl-chat-python-1.4.9/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.8/src/core/websocket.py` & `pwl-chat-python-1.4.9/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.8/src/main.py` & `pwl-chat-python-1.4.9/src/main.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.8/src/utils/utils.py` & `pwl-chat-python-1.4.9/src/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 COMMAND_GUIDE = '''
 [#cli] 进入命令交互模式
 [#chatroom] 进入聊天室模式
 [#rp] 1128 1个128积分 (默认5个,128积分)拼手气红包
 [#rp-ave] 1128 1个128积分 (默认5个,32积分)平均红包
 [#rp-hb] 5128 5个128积分 (默认5个,32积分)心跳红包
 [#rp-rps] 0128 128积分 (0=石头 1=剪刀 2=布)猜拳红包
+[#rp-rps-limit] 100 (猜拳红包超过100的不抢)
 [#rp-to] 32 Gakkiyomi,xiaoIce (积分 用户)专属红包
 [#rp-time] 3 设置抢红包等待时间
 [#bm] 发送清风明月
+[#api-key] 打印apikey
 [#answer] 进入|退出 答题模式
 [#checked] 查看当前是否签到
 [#reward] 领取昨日活跃奖励
 [#transfer] 32 Gakkiyomi 送给你 (积分 用户 留言)
 [#point] 查看当前个人积分
 [#online-users] 查看当前在线的用户列表
 [#user username] 输入 #user 用户名 可查看此用户详细信息 (#user Gakkiyomi)
```

