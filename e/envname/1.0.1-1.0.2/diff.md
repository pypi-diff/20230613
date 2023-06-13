# Comparing `tmp/envname-1.0.1.tar.gz` & `tmp/envname-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envname-1.0.1.tar", last modified: Tue May  2 04:12:13 2023, max compression
+gzip compressed data, was "envname-1.0.2.tar", last modified: Tue Jun 13 15:50:35 2023, max compression
```

## Comparing `envname-1.0.1.tar` & `envname-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 envname-1.0.1/LICENSE
--rw-r--r--   0        0        0     2002 2023-05-02 04:02:42.281502 envname-1.0.1/README.md
--rw-r--r--   0        0        0      645 2023-05-01 16:30:31.499496 envname-1.0.1/envname/__init__.py
--rw-r--r--   0        0        0      102 2023-05-01 17:24:53.385434 envname-1.0.1/envname/_envname.py
--rw-r--r--   0        0        0      583 2023-05-02 04:10:22.583936 envname-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2286 1970-01-01 00:00:00.000000 envname-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 envname-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2137 2023-06-13 15:29:36.474108 envname-1.0.2/README.md
+-rw-r--r--   0        0        0      645 2023-05-01 16:30:31.499496 envname-1.0.2/envname/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-01 17:24:53.385434 envname-1.0.2/envname/_envname.py
+-rw-r--r--   0        0        0      583 2023-06-13 15:50:31.479672 envname-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 envname-1.0.2/PKG-INFO
```

### Comparing `envname-1.0.1/LICENSE` & `envname-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `envname-1.0.1/README.md` & `envname-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # 项目描述
 
 为运行环境设置名称。
 
-有时候，对于某些功能，我们也许希望在不同的环境上采用不同的方案。以访问数据库为例：当程序在外网运行时，须通过数据库公网ip访问；而当程序在内网运行时，我们可以通过数据库内网ip访问以提高性能。
+有时候，对于某些功能，我们也许希望在不同的环境上采用不同的方案。以访问数据库为例：当程序在外网运行时，须通过数据库公网ip访问；而当程序在内网运行时，为了提高性能，我们可以通过数据库内网ip访问。
 
 # 安装
 
 ```
 pip install envname
 ```
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
+开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
 
 # 教程
 
-### 创建环境名称
+#### 创建环境名称
 
 （cmd）：
 
 ```
 envname set new_name
 ```
 
@@ -38,29 +38,29 @@
 
 1、名称不能包含空格和引号。
 
 2、名称可以包含中文。
 
 3、名称不限长度。
 
-### 查看环境名称
+#### 查看环境名称
 
 （cmd）：
 
 ```
 envname read
 ```
 
-### 导入环境名称
+#### 导入环境名称
 
 ```python
 from envname import envname
 ```
 
-### 示例
+#### 示例
 
 ```python
 import pymysql
 from envname import envname
 
 if envname == 'aliyun_HongKong_No1':
     host = '192.168.0.127'
@@ -72,8 +72,8 @@
 
 # 支持作者1元
 
 envname 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `envname-1.0.1/envname/__init__.py` & `envname-1.0.2/envname/__init__.py`

 * *Files identical despite different names*

### Comparing `envname-1.0.1/pyproject.toml` & `envname-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "envname"
-version = "1.0.1"
+version = "1.0.2"
 description = "为运行环境设置名称"
 dependencies = []
 keywords = []
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `envname-1.0.1/PKG-INFO` & `envname-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: envname
-Version: 1.0.1
+Version: 1.0.2
 Summary: 为运行环境设置名称
 Keywords: 
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/envname#readme
 
 # 项目描述
 
 为运行环境设置名称。
 
-有时候，对于某些功能，我们也许希望在不同的环境上采用不同的方案。以访问数据库为例：当程序在外网运行时，须通过数据库公网ip访问；而当程序在内网运行时，我们可以通过数据库内网ip访问以提高性能。
+有时候，对于某些功能，我们也许希望在不同的环境上采用不同的方案。以访问数据库为例：当程序在外网运行时，须通过数据库公网ip访问；而当程序在内网运行时，为了提高性能，我们可以通过数据库内网ip访问。
 
 # 安装
 
 ```
 pip install envname
 ```
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
+开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
 
 # 教程
 
-### 创建环境名称
+#### 创建环境名称
 
 （cmd）：
 
 ```
 envname set new_name
 ```
 
@@ -49,29 +49,29 @@
 
 1、名称不能包含空格和引号。
 
 2、名称可以包含中文。
 
 3、名称不限长度。
 
-### 查看环境名称
+#### 查看环境名称
 
 （cmd）：
 
 ```
 envname read
 ```
 
-### 导入环境名称
+#### 导入环境名称
 
 ```python
 from envname import envname
 ```
 
-### 示例
+#### 示例
 
 ```python
 import pymysql
 from envname import envname
 
 if envname == 'aliyun_HongKong_No1':
     host = '192.168.0.127'
@@ -83,9 +83,9 @@
 
 # 支持作者1元
 
 envname 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

