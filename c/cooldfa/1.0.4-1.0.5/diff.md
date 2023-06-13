# Comparing `tmp/cooldfa-1.0.4.tar.gz` & `tmp/cooldfa-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooldfa-1.0.4.tar", last modified: Mon May  1 01:59:35 2023, max compression
+gzip compressed data, was "cooldfa-1.0.5.tar", last modified: Tue Jun 13 15:47:02 2023, max compression
```

## Comparing `cooldfa-1.0.4.tar` & `cooldfa-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 cooldfa-1.0.4/LICENSE
--rw-r--r--   0        0        0     1985 2023-04-19 04:33:25.482492 cooldfa-1.0.4/README.md
--rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.4/cooldfa/__init__.py
--rw-r--r--   0        0        0     3661 2023-04-30 01:06:28.124524 cooldfa-1.0.4/cooldfa/_cooldfa.py
--rw-r--r--   0        0        0   478756 2023-04-30 19:24:41.305728 cooldfa-1.0.4/cooldfa/_words/others.json
--rw-r--r--   0        0        0    23188 2023-04-30 19:24:41.308762 cooldfa-1.0.4/cooldfa/_words/politics.json
--rw-r--r--   0        0        0    10325 2023-04-30 19:24:41.311777 cooldfa-1.0.4/cooldfa/_words/sex.json
--rw-r--r--   0        0        0   262857 2023-04-30 19:24:41.330728 cooldfa-1.0.4/cooldfa/_words/url.json
--rw-r--r--   0        0        0     4015 2023-04-30 19:24:41.331729 cooldfa-1.0.4/cooldfa/_words/violence.json
--rw-r--r--   0        0        0      563 2023-04-30 19:18:37.533160 cooldfa-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 cooldfa-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 cooldfa-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2118 2023-06-13 15:29:36.475109 cooldfa-1.0.5/README.md
+-rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.5/cooldfa/__init__.py
+-rw-r--r--   0        0        0     3661 2023-04-30 01:06:28.124524 cooldfa-1.0.5/cooldfa/_cooldfa.py
+-rw-r--r--   0        0        0   478756 2023-04-30 19:24:41.305728 cooldfa-1.0.5/cooldfa/_words/others.json
+-rw-r--r--   0        0        0    23188 2023-04-30 19:24:41.308762 cooldfa-1.0.5/cooldfa/_words/politics.json
+-rw-r--r--   0        0        0    10325 2023-04-30 19:24:41.311777 cooldfa-1.0.5/cooldfa/_words/sex.json
+-rw-r--r--   0        0        0   262857 2023-04-30 19:24:41.330728 cooldfa-1.0.5/cooldfa/_words/url.json
+-rw-r--r--   0        0        0     4015 2023-04-30 19:24:41.331729 cooldfa-1.0.5/cooldfa/_words/violence.json
+-rw-r--r--   0        0        0      559 2023-06-13 15:46:56.960978 cooldfa-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 cooldfa-1.0.5/PKG-INFO
```

### Comparing `cooldfa-1.0.4/LICENSE` & `cooldfa-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.4/README.md` & `cooldfa-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 # 项目描述
 
-一个基于DFA算法的敏感词检测器。
+基于 DFA 算法的敏感词检测器。
 
 # 安装
 
 ```
 pip install cooldfa
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
 
-导入：
+#### 导入
 
 ```python
 from cooldfa import dfa
 ```
 
-创建dfa模型：
+#### 创建dfa模型
 
 ```python
 敏感词S = ['123', '56', 'end']
 example = dfa(敏感词S)
 ```
 
-查找第1个敏感词：
+#### 查找第1个敏感词
 
 ```python
 example.find_one('1--2--3--4--5--6--7--8--9--end--')
 # >>> '1--2--3'
 ```
 
-查找所有敏感词：
+#### 查找所有敏感词
 
 ```python
 example.find_all('1--2--3--4--5--6--7--8--9--end--')
 # >>> ['1--2--3', '5--6', 'end']
 ```
 
-替换所有敏感词：
+#### 替换所有敏感词
 
 ```python
 example.sub('1--2--3--4--5--6--7--8--9--end--', '*')
 # >>> '*******--4--****--7--8--9--***--'
 ```
 
-使用预置的敏感词库：
+#### 使用预置的敏感词库
 
 ```python
 from cooldfa import dfa, preset_words
 
 example = dfa(
     preset_words.politics,  # 政治类
     preset_words.sex,  # 色情类
@@ -74,8 +74,8 @@
 
 # 支持作者1元
 
 cooldfa 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `cooldfa-1.0.4/cooldfa/_cooldfa.py` & `cooldfa-1.0.5/cooldfa/_cooldfa.py`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.4/cooldfa/_words/others.json` & `cooldfa-1.0.5/cooldfa/_words/others.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.4/cooldfa/_words/politics.json` & `cooldfa-1.0.5/cooldfa/_words/politics.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.4/cooldfa/_words/sex.json` & `cooldfa-1.0.5/cooldfa/_words/sex.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.4/cooldfa/_words/url.json` & `cooldfa-1.0.5/cooldfa/_words/url.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.4/cooldfa/_words/violence.json` & `cooldfa-1.0.5/cooldfa/_words/violence.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.4/pyproject.toml` & `cooldfa-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "cooldfa"
-version = "1.0.4"
-description = "一个基于DFA算法的敏感词检测器"
+version = "1.0.5"
+description = "基于 DFA 算法的敏感词检测器"
 dependencies = []
 keywords = ["cooldfa", "dfa"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

