# Comparing `tmp/rstyleslice-1.4.1.tar.gz` & `tmp/rstyleslice-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstyleslice-1.4.1.tar", last modified: Mon May  1 02:02:15 2023, max compression
+gzip compressed data, was "rstyleslice-1.4.2.tar", last modified: Tue Jun 13 15:52:03 2023, max compression
```

## Comparing `rstyleslice-1.4.1.tar` & `rstyleslice-1.4.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.4.1/LICENSE
--rw-r--r--   0        0        0     3373 2023-05-01 01:52:54.980777 rstyleslice-1.4.1/README.md
--rw-r--r--   0        0        0      589 2023-04-30 19:31:48.020869 rstyleslice-1.4.1/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4.1/rstyleslice.py
--rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 rstyleslice-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.4.2/LICENSE
+-rw-r--r--   0        0        0     3510 2023-06-13 15:29:36.465110 rstyleslice-1.4.2/README.md
+-rw-r--r--   0        0        0      591 2023-06-13 15:52:00.553142 rstyleslice-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4.2/rstyleslice.py
+-rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 rstyleslice-1.4.2/PKG-INFO
```

### Comparing `rstyleslice-1.4.1/LICENSE` & `rstyleslice-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rstyleslice-1.4.1/README.md` & `rstyleslice-1.4.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,67 +14,67 @@
 
 安装：`pip install rstyleslice`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/docs/doc.md)
 
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
 
 # 教程预览
 
-导入：
+#### 导入
 
 ```python
 from rstyleslice import rslice
 ```
 
-创建R风格容器：
+#### 创建R风格容器
 
 ```python
 obj = rslice([1,2,3,4,5,6,7,8,9])
 
 # Python中任何可以索引和切片的对象（如list、str、tuple）都可以转化成R风格容器。
 ```
 
-索引取值：
+#### 索引取值
 
 ```python
 obj[1]
 # >>> 1
 ```
 
-索引赋值：
+#### 索引赋值
 
 ```python
 obj[1] = 111
 obj[:]
 # >>> [111, 2, 3, 4, 5, 6, 7, 8, 9]
 ```
 
-切片取值：
+#### 切片取值
 
 ```python
 obj[3:7]  # >>> [3, 4, 5, 6, 7]
 obj[7:3]  # >>> [7, 6, 5, 4, 3]
 obj[3:7:2]  # >>> [3, 5, 7]
 obj[8:2:3]  # >>> [8, 5, 2]
 ```
 
-切片赋值：
+#### 切片赋值
 
 ```python
 obj[4:6] = [44, 55]
 obj[:]
 # >>> [111, 2, 3, 44, 55, 7, 8, 9]
 
 obj[4:6] = []
@@ -92,8 +92,8 @@
 
 # 支持作者1元
 
 rstyleslice 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `rstyleslice-1.4.1/pyproject.toml` & `rstyleslice-1.4.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "rstyleslice"
-version = "1.4.1"
+version = "1.4.2"
 description = "一套符合直觉的索引和切片语法"
-dependencies = ["lccpy >=1.3"]
+dependencies = ["lccpy >=1.4.7"]
 keywords = ["rstyleslice", "slice"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `rstyleslice-1.4.1/PKG-INFO` & `rstyleslice-1.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rstyleslice
-Version: 1.4.1
+Version: 1.4.2
 Summary: 一套符合直觉的索引和切片语法
 Keywords: rstyleslice,slice
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.3
+Requires-Dist: lccpy >=1.4.7
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/rstyleslice#readme
 
 # 项目描述
 
 一套符合直觉的索引和切片语法。
 
 |                                        | **Python**                                                           | **rstyleslice**                                                      |
@@ -26,67 +26,67 @@
 
 安装：`pip install rstyleslice`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/docs/doc.md)
 
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
 
 # 教程预览
 
-导入：
+#### 导入
 
 ```python
 from rstyleslice import rslice
 ```
 
-创建R风格容器：
+#### 创建R风格容器
 
 ```python
 obj = rslice([1,2,3,4,5,6,7,8,9])
 
 # Python中任何可以索引和切片的对象（如list、str、tuple）都可以转化成R风格容器。
 ```
 
-索引取值：
+#### 索引取值
 
 ```python
 obj[1]
 # >>> 1
 ```
 
-索引赋值：
+#### 索引赋值
 
 ```python
 obj[1] = 111
 obj[:]
 # >>> [111, 2, 3, 4, 5, 6, 7, 8, 9]
 ```
 
-切片取值：
+#### 切片取值
 
 ```python
 obj[3:7]  # >>> [3, 4, 5, 6, 7]
 obj[7:3]  # >>> [7, 6, 5, 4, 3]
 obj[3:7:2]  # >>> [3, 5, 7]
 obj[8:2:3]  # >>> [8, 5, 2]
 ```
 
-切片赋值：
+#### 切片赋值
 
 ```python
 obj[4:6] = [44, 55]
 obj[:]
 # >>> [111, 2, 3, 44, 55, 7, 8, 9]
 
 obj[4:6] = []
@@ -104,9 +104,9 @@
 
 # 支持作者1元
 
 rstyleslice 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

