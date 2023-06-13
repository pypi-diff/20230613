# Comparing `tmp/encrypt256-1.8.2.tar.gz` & `tmp/encrypt256-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encrypt256-1.8.2.tar", last modified: Mon May  1 02:00:52 2023, max compression
+gzip compressed data, was "encrypt256-1.8.3.tar", last modified: Tue Jun 13 15:50:01 2023, max compression
```

## Comparing `encrypt256-1.8.2.tar` & `encrypt256-1.8.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-14 11:47:56.900367 encrypt256-1.8.2/LICENSE
--rw-r--r--   0        0        0     2373 2023-04-29 18:08:03.699670 encrypt256-1.8.2/README.md
--rw-r--r--   0        0        0       30 2023-04-10 04:00:30.884575 encrypt256-1.8.2/encrypt256.py
--rw-r--r--   0        0        0      632 2023-04-30 19:28:40.636989 encrypt256-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 encrypt256-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-14 11:47:56.900367 encrypt256-1.8.3/LICENSE
+-rw-r--r--   0        0        0     2491 2023-06-13 15:29:36.475109 encrypt256-1.8.3/README.md
+-rw-r--r--   0        0        0       30 2023-04-10 04:00:30.884575 encrypt256-1.8.3/encrypt256.py
+-rw-r--r--   0        0        0      616 2023-06-13 15:49:57.671735 encrypt256-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 encrypt256-1.8.3/PKG-INFO
```

### Comparing `encrypt256-1.8.2/LICENSE` & `encrypt256-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `encrypt256-1.8.2/README.md` & `encrypt256-1.8.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 # 项目描述
 
-一个用于加密str型和bytes型数据的加密器。
+str 型和 bytes 型数据加密器。
 
-1、底层加密算法为AES-CBC-256。
+1、底层加密算法为 AES-CBC-256。
 
-2、加密时，会自动创建随机salt、随机iv、原始明文的校验值，并把校验值添加到密文中。
+2、加密时，会自动创建随机 salt、随机 iv、原始明文的校验值，并把校验值添加到密文中。
 
 3、解密时，会自动根据校验值校验“解密得到的明文”与“原始明文”是否一致。
 
 # 安装
 
 ```
 pip install encrypt256
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
 
-### 导入
+#### 导入
 
 ```python
 from encrypt256 import Encrypt256
 ```
 
-### 创建加密器
+#### 创建加密器
 
 ```python
 password1 = 123456789  # 支持int型密钥
 password2 = '黄河之水天上来'  # 支持str型密钥
 password3 = '床前明月光'.encode('utf8')  # 支持bytes型密钥
 
 enctool = Encrypt256(password1)  # 创建加密器
 ```
 
-### 加密
+#### 加密
 
 ```python
 p1 = '人生自古谁五死'  # 可加密str型数据
 p2 = '莎士比亚'.encode('utf8')  # 可加密bytes型数据
 
 c1 = enctool.encrypt(p1)
 c2 = enctool.encrypt(p2)
 ```
 
-### 解密
+#### 解密
 
 ```python
 r1 = enctool.decrypt(c1)
 r2 = enctool.decrypt(c2)
 
 assert p1 == r1
 assert p2 == r2
@@ -68,18 +68,18 @@
 assert type(p2) is type(r2)
 ```
 
 当发生以下情况时，会解密失败并报错：
 
 1、密钥错误。
 
-2、由于密文被篡改，导致AES算法解密失败。
+2、由于密文被篡改，导致 AES 算法解密失败。
 
-3、由于密文被篡改，虽然AES算法解密成功，但校验值错误。
+3、由于密文被篡改，虽然 AES 算法解密成功，但校验值错误。
 
 # 支持作者1元
 
 encrypt256 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `encrypt256-1.8.2/pyproject.toml` & `encrypt256-1.8.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "encrypt256"
-version = "1.8.2"
-description = "一个用于加密str型和bytes型数据的加密器"
-dependencies = ["lccpy >=1.3"]
+version = "1.8.3"
+description = "str 型和 bytes 型数据加密器"
+dependencies = ["lccpy >=1.4.7"]
 keywords = ["encrypt256", "encrypt", "AES", "pycryptodome", "Crypto"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `encrypt256-1.8.2/PKG-INFO` & `encrypt256-1.8.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: encrypt256
-Version: 1.8.2
-Summary: 一个用于加密str型和bytes型数据的加密器
+Version: 1.8.3
+Summary: str 型和 bytes 型数据加密器
 Keywords: encrypt256,encrypt,AES,pycryptodome,Crypto
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.3
+Requires-Dist: lccpy >=1.4.7
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/encrypt256#readme
 
 # 项目描述
 
-一个用于加密str型和bytes型数据的加密器。
+str 型和 bytes 型数据加密器。
 
-1、底层加密算法为AES-CBC-256。
+1、底层加密算法为 AES-CBC-256。
 
-2、加密时，会自动创建随机salt、随机iv、原始明文的校验值，并把校验值添加到密文中。
+2、加密时，会自动创建随机 salt、随机 iv、原始明文的校验值，并把校验值添加到密文中。
 
 3、解密时，会自动根据校验值校验“解密得到的明文”与“原始明文”是否一致。
 
 # 安装
 
 ```
 pip install encrypt256
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
 
-### 导入
+#### 导入
 
 ```python
 from encrypt256 import Encrypt256
 ```
 
-### 创建加密器
+#### 创建加密器
 
 ```python
 password1 = 123456789  # 支持int型密钥
 password2 = '黄河之水天上来'  # 支持str型密钥
 password3 = '床前明月光'.encode('utf8')  # 支持bytes型密钥
 
 enctool = Encrypt256(password1)  # 创建加密器
 ```
 
-### 加密
+#### 加密
 
 ```python
 p1 = '人生自古谁五死'  # 可加密str型数据
 p2 = '莎士比亚'.encode('utf8')  # 可加密bytes型数据
 
 c1 = enctool.encrypt(p1)
 c2 = enctool.encrypt(p2)
 ```
 
-### 解密
+#### 解密
 
 ```python
 r1 = enctool.decrypt(c1)
 r2 = enctool.decrypt(c2)
 
 assert p1 == r1
 assert p2 == r2
@@ -80,19 +80,19 @@
 assert type(p2) is type(r2)
 ```
 
 当发生以下情况时，会解密失败并报错：
 
 1、密钥错误。
 
-2、由于密文被篡改，导致AES算法解密失败。
+2、由于密文被篡改，导致 AES 算法解密失败。
 
-3、由于密文被篡改，虽然AES算法解密成功，但校验值错误。
+3、由于密文被篡改，虽然 AES 算法解密成功，但校验值错误。
 
 # 支持作者1元
 
 encrypt256 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

