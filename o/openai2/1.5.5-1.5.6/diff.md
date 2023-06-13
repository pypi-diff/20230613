# Comparing `tmp/openai2-1.5.5.tar.gz` & `tmp/openai2-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.5.tar", last modified: Sun May 28 04:57:48 2023, max compression
+gzip compressed data, was "openai2-1.5.6.tar", last modified: Tue Jun 13 15:51:38 2023, max compression
```

## Comparing `openai2-1.5.5.tar` & `openai2-1.5.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.5/LICENSE
--rw-r--r--   0        0        0     2866 2023-05-28 04:47:47.511099 openai2-1.5.5/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.5/openai2/Licenses of dependent packages/openai/LICENSE
--rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.5/openai2/__init__.py
--rw-r--r--   0        0        0     2577 2023-05-28 04:22:51.712836 openai2-1.5.5/openai2/openai2.py
--rw-r--r--   0        0        0      634 2023-05-28 04:50:00.858650 openai2-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 openai2-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.6/LICENSE
+-rw-r--r--   0        0        0     2944 2023-06-13 15:29:36.465110 openai2-1.5.6/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.6/openai2/Licenses of dependent packages/openai/LICENSE
+-rw-r--r--   0        0        0       23 2023-05-28 06:12:32.856591 openai2-1.5.6/openai2/__init__.py
+-rw-r--r--   0        0        0     2576 2023-05-28 05:05:03.581780 openai2-1.5.6/openai2/_core.py
+-rw-r--r--   0        0        0      633 2023-06-13 15:51:17.749084 openai2-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 openai2-1.5.6/PKG-INFO
```

### Comparing `openai2-1.5.5/LICENSE` & `openai2-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.5/README.md` & `openai2-1.5.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,55 +12,55 @@
 
 [获取链接1](https://platform.openai.com/account/api-keys)
 
 [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
 
 # 教程
 
-##### 导入
+#### 导入
 
 ```python
 from openai2 import Chat
 ```
 
-##### 创建对话
+#### 创建对话
 
 ```python
 api_key = 'api_key'  # 更换成自己的api_key
 
 Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
 Lucy = Chat(api_key=api_key, model="gpt-3.5-turbo")  # 每个实例可使用 相同 或者 不同 的api_key
 ```
 
-##### 对话
+#### 对话
 
 ```python
 Tony.request('数字1的后面是几?')  # >>> 2
 Lucy.request('数字101的后面是几?')  # >>> 102
 
 Tony.request('再往后是几?')  # >>> 3
 Lucy.request('再往后是几?')  # >>> 103
 ```
 
-##### 存档
+#### 存档
 
 ```python
 Tony.dump('./talk_record.json')
 ```
 
-##### 载入存档
+#### 载入存档
 
 ```python
 Jenny = Chat(api_key=api_key, model="gpt-3.5-turbo")
 Jenny.load('./talk_record.json')
 
 Jenny.request('再往后呢?')  # >>> 4
 ```
 
-##### 对话回滚
+#### 对话回滚
 
 ```python
 Anna = Chat(api_key=api_key, model="gpt-3.5-turbo")
 
 Anna.request('数字1的后面是几?')  # >>> 2
 Anna.request('再往后是几?')  # >>> 3
 Anna.request('再往后呢?')  # >>> 4
@@ -72,32 +72,34 @@
 Anna.rollback()  # >>> [user]:数字1的后面是几?  [assistant]:2
 
 Anna.request('再往后是几?')  # >>> 3
 ```
 
 注：
 
-执行1次 `Anna.rollback(n=10)` 等效于执行10次 `Anna.rollback()`  。
+执行1次 `Anna.rollback(n=x)` 等效于执行x次 `Anna.rollback()`  ，例如：
 
-##### 修改api_key
+执行1次 `Anna.rollback(n=5)` 等效于执行5次 `Anna.rollback()`  。
+
+#### 修改api_key
 
 ```python
 Anna.api_key = 'new api_key'
 ```
 
-##### 更多方法
+#### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQR-max.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
+开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
```

### Comparing `openai2-1.5.5/openai2/Licenses of dependent packages/openai/LICENSE` & `openai2-1.5.6/openai2/Licenses of dependent packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.5/openai2/openai2.py` & `openai2-1.5.6/openai2/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.model = model
         self.messages = []
         self.kwargs = kwargs
 
     def rollback(self, n=1):
         self.messages[-2*n:] = []
         for x in self.messages[-2:]:
-            print(f"[{x['role']}]: {x['content']}")
+            print(f"[{x['role']}]:{x['content']}")
     
     def request(self, text:str):
         completion = openai.ChatCompletion.create(**{
             'api_key': self.api_key,
             'model': self.model,
             'messages': self.messages + [{"role": "user", "content": text}],
             **self.kwargs
```

### Comparing `openai2-1.5.5/pyproject.toml` & `openai2-1.5.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.5.5"
-description = "根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。"
+version = "1.5.6"
+description = "根据 openai 官方接口‘openai’改造的‘openai2’，比官方接口更好用一点"
 dependencies = ["openai >=0.27.0"]
 keywords = ["openai2", "openai"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `openai2-1.5.5/PKG-INFO` & `openai2-1.5.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.5
-Summary: 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
+Version: 1.5.6
+Summary: 根据 openai 官方接口‘openai’改造的‘openai2’，比官方接口更好用一点
 Keywords: openai2,openai
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/openai2#readme
@@ -24,55 +24,55 @@
 
 [获取链接1](https://platform.openai.com/account/api-keys)
 
 [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
 
 # 教程
 
-##### 导入
+#### 导入
 
 ```python
 from openai2 import Chat
 ```
 
-##### 创建对话
+#### 创建对话
 
 ```python
 api_key = 'api_key'  # 更换成自己的api_key
 
 Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
 Lucy = Chat(api_key=api_key, model="gpt-3.5-turbo")  # 每个实例可使用 相同 或者 不同 的api_key
 ```
 
-##### 对话
+#### 对话
 
 ```python
 Tony.request('数字1的后面是几?')  # >>> 2
 Lucy.request('数字101的后面是几?')  # >>> 102
 
 Tony.request('再往后是几?')  # >>> 3
 Lucy.request('再往后是几?')  # >>> 103
 ```
 
-##### 存档
+#### 存档
 
 ```python
 Tony.dump('./talk_record.json')
 ```
 
-##### 载入存档
+#### 载入存档
 
 ```python
 Jenny = Chat(api_key=api_key, model="gpt-3.5-turbo")
 Jenny.load('./talk_record.json')
 
 Jenny.request('再往后呢?')  # >>> 4
 ```
 
-##### 对话回滚
+#### 对话回滚
 
 ```python
 Anna = Chat(api_key=api_key, model="gpt-3.5-turbo")
 
 Anna.request('数字1的后面是几?')  # >>> 2
 Anna.request('再往后是几?')  # >>> 3
 Anna.request('再往后呢?')  # >>> 4
@@ -84,33 +84,35 @@
 Anna.rollback()  # >>> [user]:数字1的后面是几?  [assistant]:2
 
 Anna.request('再往后是几?')  # >>> 3
 ```
 
 注：
 
-执行1次 `Anna.rollback(n=10)` 等效于执行10次 `Anna.rollback()`  。
+执行1次 `Anna.rollback(n=x)` 等效于执行x次 `Anna.rollback()`  ，例如：
 
-##### 修改api_key
+执行1次 `Anna.rollback(n=5)` 等效于执行5次 `Anna.rollback()`  。
+
+#### 修改api_key
 
 ```python
 Anna.api_key = 'new api_key'
 ```
 
-##### 更多方法
+#### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQR-max.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
+开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
```

