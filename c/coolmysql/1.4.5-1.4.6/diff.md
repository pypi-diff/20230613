# Comparing `tmp/coolmysql-1.4.5.tar.gz` & `tmp/coolmysql-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.4.5.tar", last modified: Mon May  1 02:00:29 2023, max compression
+gzip compressed data, was "coolmysql-1.4.6.tar", last modified: Tue Jun 13 15:47:55 2023, max compression
```

## Comparing `coolmysql-1.4.5.tar` & `coolmysql-1.4.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.5/LICENSE
--rw-r--r--   0        0        0     4261 2023-05-01 01:52:37.715384 coolmysql-1.4.5/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.5/coolmysql.py
--rw-r--r--   0        0        0      582 2023-04-30 19:28:27.619336 coolmysql-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 coolmysql-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.6/LICENSE
+-rw-r--r--   0        0        0     4427 2023-06-13 15:29:36.475109 coolmysql-1.4.6/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.6/coolmysql.py
+-rw-r--r--   0        0        0      601 2023-06-13 15:47:52.295261 coolmysql-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 coolmysql-1.4.6/PKG-INFO
```

### Comparing `coolmysql-1.4.5/LICENSE` & `coolmysql-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4.5/README.md` & `coolmysql-1.4.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 
 安装：`pip install coolmysql`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/docs/doc.md)
 
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
 from pymysql import connect
 from coolmysql import ORM, mc, mf
 ```
 
-创建ORM：
+#### 创建ORM
 
 ```python
 def mkconn():
     return connect(
         host = 'localhost',
         port = 3306,
         user = 'root',
@@ -43,93 +43,95 @@
     )
 
 orm = ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
-新增数据：
+#### 新增数据
 
 ```python
 line1 = {'姓名': '小一', '年龄':11, '签到日期':'2023-01-11'}
 line2 = {'姓名': '小二', '年龄':12, '签到日期':'2023-01-12'}
 line3 = {'姓名': '小三', '年龄':13, '签到日期':'2023-01-13'}
 line4 = {'姓名': '小四', '年龄':14, '签到日期':'2023-01-14'}
 line5 = {'姓名': '小五', '年龄':15, '签到日期':'2023-01-15'}
 line6 = {'姓名': '小六', '年龄':16, '签到日期':'2023-01-16'}
 
 r1 = sheet + line1  # 添加1条数据
 r2 = sheet + [line2, line3, line4, line5, line6]  # 批量添加
 ```
 
-查询：
+#### 查询
 
 ```python
 sheet[:]  # 查询所有数据
 
 sheet[3]  # 查询第3条数据
 
 sheet[mc.年龄>13][mc.姓名=='小五'][1]  # 查询年龄大于13、且姓名叫'小五'的第1条数据
 ```
 
-修改：
+#### 修改
 
 ```python
 sheet[mc.年龄>10][2:5] = {
     '视力': 5.0,
     '性别': '男',
     '爱好': '足球, 篮球, 画画, 跳绳'
 }
 ```
 
-删除：
+#### 删除
 
 ```python
 # 删除年龄>=15的所有数据
 sheet[mc.年龄>=15][:] = None
 
 # 删除年龄大于10、且喜欢足球的第2条数据
 sheet[mc.年龄>10][mc.爱好.re('足球')][2] = None
 
 # 删除所有数据
 sheet[:] = None
 ```
 
-比较运算：
+#### 比较运算
 
 | **代码** |
 | -------------- |
 | mc.年龄 > 10   |
 | mc.年龄 >= 10  |
 | mc.年龄 < 10   |
 | ...            |
 
-成员运算：
+#### 成员运算
 
 | **代码**               | **解释**                   |
 | ---------------------------- | -------------------------------- |
 | mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
 | mc.年龄.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
 
-过滤器的集合运算：
+#### 过滤器的集合运算
 
 | **代码**                                                         | **解释** |
 | ---------------------------------------------------------------------- | -------------- |
 | [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
 | [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
 | [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
 | [ ~(mc.年龄>100) ]                                                     | 补集           |
 
+#### 限定字段
+
 只返回姓名、年龄这2个字段：
 
 ```python
 sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
-执行原生SQL语句：
+#### 执行原生SQL语句
 
 ```python
 data, cursor = sheet.execute('select 姓名 from 希望小学 limit 1')
 data
 # >>> [{'姓名': '小一'}]
 
 data, cursor = sheet.execute('update 希望小学 set 爱好="Python" limit 3')
@@ -139,8 +141,8 @@
 
 # 支持作者1元
 
 coolmysql 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `coolmysql-1.4.5/pyproject.toml` & `coolmysql-1.4.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmysql"
-version = "1.4.5"
+version = "1.4.6"
 description = "史上最优雅的 mysql ORM"
-dependencies = ["lccpy >=1.4.5"]
-keywords = ["coolmysql", "pymysql", "mysql"]
+dependencies = ["lccpy >=1.4.7"]
+keywords = ["coolmysql", "pymysql", "mysql", "aiomysql", "orm"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `coolmysql-1.4.5/PKG-INFO` & `coolmysql-1.4.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.4.5
+Version: 1.4.6
 Summary: 史上最优雅的 mysql ORM
-Keywords: coolmysql,pymysql,mysql
+Keywords: coolmysql,pymysql,mysql,aiomysql,orm
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.5
+Requires-Dist: lccpy >=1.4.7
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmysql#readme
 
 # 项目描述
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmysql`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/docs/doc.md)
 
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
 from pymysql import connect
 from coolmysql import ORM, mc, mf
 ```
 
-创建ORM：
+#### 创建ORM
 
 ```python
 def mkconn():
     return connect(
         host = 'localhost',
         port = 3306,
         user = 'root',
@@ -55,93 +55,95 @@
     )
 
 orm = ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
-新增数据：
+#### 新增数据
 
 ```python
 line1 = {'姓名': '小一', '年龄':11, '签到日期':'2023-01-11'}
 line2 = {'姓名': '小二', '年龄':12, '签到日期':'2023-01-12'}
 line3 = {'姓名': '小三', '年龄':13, '签到日期':'2023-01-13'}
 line4 = {'姓名': '小四', '年龄':14, '签到日期':'2023-01-14'}
 line5 = {'姓名': '小五', '年龄':15, '签到日期':'2023-01-15'}
 line6 = {'姓名': '小六', '年龄':16, '签到日期':'2023-01-16'}
 
 r1 = sheet + line1  # 添加1条数据
 r2 = sheet + [line2, line3, line4, line5, line6]  # 批量添加
 ```
 
-查询：
+#### 查询
 
 ```python
 sheet[:]  # 查询所有数据
 
 sheet[3]  # 查询第3条数据
 
 sheet[mc.年龄>13][mc.姓名=='小五'][1]  # 查询年龄大于13、且姓名叫'小五'的第1条数据
 ```
 
-修改：
+#### 修改
 
 ```python
 sheet[mc.年龄>10][2:5] = {
     '视力': 5.0,
     '性别': '男',
     '爱好': '足球, 篮球, 画画, 跳绳'
 }
 ```
 
-删除：
+#### 删除
 
 ```python
 # 删除年龄>=15的所有数据
 sheet[mc.年龄>=15][:] = None
 
 # 删除年龄大于10、且喜欢足球的第2条数据
 sheet[mc.年龄>10][mc.爱好.re('足球')][2] = None
 
 # 删除所有数据
 sheet[:] = None
 ```
 
-比较运算：
+#### 比较运算
 
 | **代码** |
 | -------------- |
 | mc.年龄 > 10   |
 | mc.年龄 >= 10  |
 | mc.年龄 < 10   |
 | ...            |
 
-成员运算：
+#### 成员运算
 
 | **代码**               | **解释**                   |
 | ---------------------------- | -------------------------------- |
 | mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
 | mc.年龄.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
 
-过滤器的集合运算：
+#### 过滤器的集合运算
 
 | **代码**                                                         | **解释** |
 | ---------------------------------------------------------------------- | -------------- |
 | [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
 | [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
 | [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
 | [ ~(mc.年龄>100) ]                                                     | 补集           |
 
+#### 限定字段
+
 只返回姓名、年龄这2个字段：
 
 ```python
 sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
-执行原生SQL语句：
+#### 执行原生SQL语句
 
 ```python
 data, cursor = sheet.execute('select 姓名 from 希望小学 limit 1')
 data
 # >>> [{'姓名': '小一'}]
 
 data, cursor = sheet.execute('update 希望小学 set 爱好="Python" limit 3')
@@ -151,9 +153,9 @@
 
 # 支持作者1元
 
 coolmysql 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

