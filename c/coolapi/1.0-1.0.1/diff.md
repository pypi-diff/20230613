# Comparing `tmp/coolapi-1.0.tar.gz` & `tmp/coolapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolapi-1.0.tar", last modified: Sat May 27 11:54:59 2023, max compression
+gzip compressed data, was "coolapi-1.0.1.tar", last modified: Tue Jun 13 15:43:39 2023, max compression
```

## Comparing `coolapi-1.0.tar` & `coolapi-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 coolapi-1.0/LICENSE
--rw-r--r--   0        0        0     5292 2023-05-27 11:40:02.442076 coolapi-1.0/README.md
--rw-r--r--   0        0        0    11358 2023-05-14 02:53:10.000000 coolapi-1.0/coolapi/Licenses of dependent packages/tornado/LICENSE
--rw-r--r--   0        0        0       43 2023-05-26 07:00:38.945694 coolapi-1.0/coolapi/__init__.py
--rw-r--r--   0        0        0     1668 2023-05-27 11:00:33.037396 coolapi-1.0/coolapi/_coolapi.py
--rw-r--r--   0        0        0      611 2023-05-27 11:28:03.719778 coolapi-1.0/pyproject.toml
--rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 coolapi-1.0/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 coolapi-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5330 2023-06-13 15:29:36.475109 coolapi-1.0.1/README.md
+-rw-r--r--   0        0        0       27 2023-06-12 17:15:32.722578 coolapi-1.0.1/coolapi.py
+-rw-r--r--   0        0        0      619 2023-06-13 15:43:29.448879 coolapi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5601 1970-01-01 00:00:00.000000 coolapi-1.0.1/PKG-INFO
```

### Comparing `coolapi-1.0/LICENSE` & `coolapi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coolapi-1.0/README.md` & `coolapi-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatSubscribeQR-max.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
+开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
 
 # 教程
 
-##### 导入
+#### 导入
 
 ```python
 import asyncio
 from coolapi import handler, creat_server
 ```
 
-##### 一个最简单的例子
+#### 一个最简单的例子
 
 ```python
 class LoginHandler(handler):
     urls = ['/login/?']
     # url必须以'/'开头
     # '?'是正则表达式语法, 相当于 urls = ['/login', '/login/']
 
@@ -53,53 +53,55 @@
 asyncio.run(main())
 
 # 此时可在浏览器访问：
 # http://localhost:5050/login
 # http://localhost:5050/login/
 ```
 
-##### 设置 cookie
+#### 设置 cookie
 
 ```python
 class PersonalHandler(handler):
     urls = ['/personal/?']
 
     async def get(self):
         self.set_cookie(name='username', value='tony')
         return self.write('Welcome to the personal center!')
 ```
 
-##### 重定向
+#### 重定向
 
 ```python
 def judge_login(self):
     ...
 
 class PersonalHandler(handler):
     urls = ['/personal/?']
 
     async def get(self):
         if judge_login(self):
             return self.write('Welcome to the personal center!')
         else:
-            return self.redirect('/login')  # 重定向到login
+            return self.redirect('/login')  # 重定向到'/login'
 ```
 
-##### 常用的视图操作
+#### 常用的视图操作
 
 | 功能         | 代码                                           |
 | ------------ | ---------------------------------------------- |
 | 返回响应     | return self.write('......')                    |
-| 设置cookie   | self.set_cookie(name='username', value='tony') |
-| 获取cookie   | self.get_cookie(name='username')               |
+| 设置 cookie  | self.set_cookie(name='username', value='tony') |
+| 获取 cookie  | self.get_cookie(name='username')               |
 | 重定向       | return self.redirect('/login')                 |
 | 获取访客ip   | ip = self.get_ip( )                            |
 | 获取请求数据 | body = self.get_body( )                        |
 
-##### 使用通配路由
+#### 使用通配路由
+
+路由支持正则表达式，因此可实现通配路由：
 
 ```python
 class ArticleHandler(handler):
     urls = ['/article/(\d+)/([a-z0-9]+)/?']
 
     async def get(self, userid, article_id):
         text = f"The article you are reading is '{article_id}' written by {userid}"
@@ -121,52 +123,52 @@
 
 # 运行后可在浏览器访问：
 # http://localhost:5050/documention/python3
 # http://localhost:5050/documention/python3.9
 # ...
 ```
 
-##### 启动 http 服务
+#### 启动 http 服务
 
 ```python
 class LoginHandler(handler):
     urls = ['/login/?']
     async def get(self):
         return self.write('You are accessing the get method of login')
 
 class ArticleHandler(handler):
     ...
 
 async def main():
     http_server = creat_server(
-      
-        handlers = [LoginHandler, ArticleHandler],  # 要注册的视图类
-      
+  
+        handlers = [LoginHandler, ArticleHandler],  # 视图类列表
+  
         port = 5050,  # 端口, 默认为80
-      
+  
         static_path = None,  # 静态文件服务, 默认为None
-      
+  
         debug = False,  # 启用调试模式, 默认为False
-      
+  
         # 支持更多参数, 可参考 https://www.tornadoweb.org/en/stable/web.html#tornado.web.Application
     )
   
     await asyncio.sleep(float('inf'))  # float('inf')表示无穷大
 
 asyncio.run(main())
 ```
 
-##### 更多用法
+#### 更多用法
 
 coolapi 是对 tornado 的二次封装，其中：
 
 1、coolapi.handler（视图类）继承自 [tornado.web.RequestHandler](https://www.tornadoweb.org/en/stable/web.html#request-handlers)，可使用 tornado.web.RequestHandler 的任何功能。
 
 2、creat_server 支持 [tornado.web.Application](https://www.tornadoweb.org/en/stable/web.html#tornado.web.Application) 的所有参数。
 
 # 支持作者1元
 
 coolapi 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-200x200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `coolapi-1.0/pyproject.toml` & `coolapi-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolapi"
-version = "1.0"
+version = "1.0.1"
 description = "简单好用的异步 web 框架"
-dependencies = ["tornado"]
+dependencies = ["lccpy >=1.4.7"]
 keywords = ["coolapi", "tornado", "flask", "fastapi", "django", "aiohttp", "web"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `coolapi-1.0/PKG-INFO` & `coolapi-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: coolapi
-Version: 1.0
+Version: 1.0.1
 Summary: 简单好用的异步 web 框架
 Keywords: coolapi,tornado,flask,fastapi,django,aiohttp,web
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: tornado
+Requires-Dist: lccpy >=1.4.7
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolapi#readme
 
 # 项目描述
 
 简单好用的异步 web 框架。
 
 # 安装
@@ -26,28 +26,28 @@
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatSubscribeQR-max.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
+开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
 
 # 教程
 
-##### 导入
+#### 导入
 
 ```python
 import asyncio
 from coolapi import handler, creat_server
 ```
 
-##### 一个最简单的例子
+#### 一个最简单的例子
 
 ```python
 class LoginHandler(handler):
     urls = ['/login/?']
     # url必须以'/'开头
     # '?'是正则表达式语法, 相当于 urls = ['/login', '/login/']
 
@@ -65,53 +65,55 @@
 asyncio.run(main())
 
 # 此时可在浏览器访问：
 # http://localhost:5050/login
 # http://localhost:5050/login/
 ```
 
-##### 设置 cookie
+#### 设置 cookie
 
 ```python
 class PersonalHandler(handler):
     urls = ['/personal/?']
 
     async def get(self):
         self.set_cookie(name='username', value='tony')
         return self.write('Welcome to the personal center!')
 ```
 
-##### 重定向
+#### 重定向
 
 ```python
 def judge_login(self):
     ...
 
 class PersonalHandler(handler):
     urls = ['/personal/?']
 
     async def get(self):
         if judge_login(self):
             return self.write('Welcome to the personal center!')
         else:
-            return self.redirect('/login')  # 重定向到login
+            return self.redirect('/login')  # 重定向到'/login'
 ```
 
-##### 常用的视图操作
+#### 常用的视图操作
 
 | 功能         | 代码                                           |
 | ------------ | ---------------------------------------------- |
 | 返回响应     | return self.write('......')                    |
-| 设置cookie   | self.set_cookie(name='username', value='tony') |
-| 获取cookie   | self.get_cookie(name='username')               |
+| 设置 cookie  | self.set_cookie(name='username', value='tony') |
+| 获取 cookie  | self.get_cookie(name='username')               |
 | 重定向       | return self.redirect('/login')                 |
 | 获取访客ip   | ip = self.get_ip( )                            |
 | 获取请求数据 | body = self.get_body( )                        |
 
-##### 使用通配路由
+#### 使用通配路由
+
+路由支持正则表达式，因此可实现通配路由：
 
 ```python
 class ArticleHandler(handler):
     urls = ['/article/(\d+)/([a-z0-9]+)/?']
 
     async def get(self, userid, article_id):
         text = f"The article you are reading is '{article_id}' written by {userid}"
@@ -133,53 +135,53 @@
 
 # 运行后可在浏览器访问：
 # http://localhost:5050/documention/python3
 # http://localhost:5050/documention/python3.9
 # ...
 ```
 
-##### 启动 http 服务
+#### 启动 http 服务
 
 ```python
 class LoginHandler(handler):
     urls = ['/login/?']
     async def get(self):
         return self.write('You are accessing the get method of login')
 
 class ArticleHandler(handler):
     ...
 
 async def main():
     http_server = creat_server(
-      
-        handlers = [LoginHandler, ArticleHandler],  # 要注册的视图类
-      
+  
+        handlers = [LoginHandler, ArticleHandler],  # 视图类列表
+  
         port = 5050,  # 端口, 默认为80
-      
+  
         static_path = None,  # 静态文件服务, 默认为None
-      
+  
         debug = False,  # 启用调试模式, 默认为False
-      
+  
         # 支持更多参数, 可参考 https://www.tornadoweb.org/en/stable/web.html#tornado.web.Application
     )
   
     await asyncio.sleep(float('inf'))  # float('inf')表示无穷大
 
 asyncio.run(main())
 ```
 
-##### 更多用法
+#### 更多用法
 
 coolapi 是对 tornado 的二次封装，其中：
 
 1、coolapi.handler（视图类）继承自 [tornado.web.RequestHandler](https://www.tornadoweb.org/en/stable/web.html#request-handlers)，可使用 tornado.web.RequestHandler 的任何功能。
 
 2、creat_server 支持 [tornado.web.Application](https://www.tornadoweb.org/en/stable/web.html#tornado.web.Application) 的所有参数。
 
 # 支持作者1元
 
 coolapi 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-200x200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

