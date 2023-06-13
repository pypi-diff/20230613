# Comparing `tmp/asymongo-1.3.2.tar.gz` & `tmp/asymongo-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymongo-1.3.2.tar", last modified: Mon May  1 01:56:11 2023, max compression
+gzip compressed data, was "asymongo-1.3.3.tar", last modified: Tue Jun 13 15:45:20 2023, max compression
```

## Comparing `asymongo-1.3.2.tar` & `asymongo-1.3.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymongo-1.3.2/LICENSE
--rw-r--r--   0        0        0     5184 2023-05-01 01:51:56.097037 asymongo-1.3.2/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3.2/asymongo.py
--rw-r--r--   0        0        0      583 2023-05-01 01:53:26.451415 asymongo-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 asymongo-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymongo-1.3.3/LICENSE
+-rw-r--r--   0        0        0     5338 2023-06-13 15:29:36.475109 asymongo-1.3.3/README.md
+-rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3.3/asymongo.py
+-rw-r--r--   0        0        0      590 2023-06-13 15:44:55.395808 asymongo-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5612 1970-01-01 00:00:00.000000 asymongo-1.3.3/PKG-INFO
```

### Comparing `asymongo-1.3.2/LICENSE` & `asymongo-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asymongo-1.3.2/README.md` & `asymongo-1.3.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,141 +6,143 @@
 
 安装：`pip install asymongo`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/docs/doc.md)
 
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
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
 import asymongo as mg
 from asymongo import mc, mup
 ```
 
-创建ORM：
+#### 创建ORM
 
 ```python
 mkconn = lambda: MongoClient(host='localhost', port=27017)
 
 orm = mg.ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
-新增数据：
+#### 新增数据
 
 ```python
 line1 = {'姓名': '小一', '年龄':11, '幸运数字':[1, 2, 3], '成绩':{'语文':81, '数学':82}}
 line2 = {'姓名': '小二', '年龄':12, '幸运数字':[2, 3, 4], '成绩':{'语文':82, '数学':83}}
 line3 = {'姓名': '小三', '年龄':13, '幸运数字':[3, 4, 5], '成绩':{'语文':83, '数学':84}}
 line4 = {'姓名': '小四', '年龄':14, '幸运数字':[4, 5, 6], '成绩':{'语文':84, '数学':85}}
 line5 = {'姓名': '小五', '年龄':15, '幸运数字':[5, 6, 7], '成绩':{'语文':85, '数学':86}}
 line6 = {'姓名': '小六', '年龄':16, '幸运数字':[6, 7, 8], '成绩':{'语文':86, '数学':87}}
 
 await sheet.insert(line1)  # 添加1条数据
 await sheet.insert([ line2, line3, line4, line5, line6 ])  # 批量添加
 ```
 
-查询：
+#### 查询
 
 ```python
 await sheet[:]  # 查询所有数据
 
 await sheet[3]  # 查询第3条数据
 
 await sheet[mc.成绩.语文 == 85][:]  # 查询语文成绩为85分的数据
 
 await sheet[mc.年龄>13][mc.姓名=='小五'][1]  # 查询年龄大于13、且姓名叫'小五'的第1条数据
 ```
 
-修改：
+#### 修改
 
 ```python
 data = {
     '视力': 5.0,
     '性别': '男',
     '爱好': ['足球','篮球','画画','跳绳'],
     '幸运数字': mup.push(15,16,17),  # 添加到列表
     '年龄': mup.inc(2)  # 自增
 }
 
 await sheet.update(data)[2:5]
 ```
 
-删除：
+#### 删除
 
 ```python
 # 删除年龄>=15的数据
 await sheet[mc.年龄>=15].delete()[:]
 
 # 删除年龄大于10、且姓名包含'小'的第2条数据
 await sheet[mc.年龄>10][mc.姓名 == mg.re('小')].delete()[2]
 
 # 删除所有数据
 await sheet.delete()[:]
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
 
 | **代码**                           | **解释**                       |
 | ---------------------------------------- | ------------------------------------ |
 | mc.年级 == mg.isin('初三', '高二')       | 若字段值是传入值的成员，则符合       |
 | mc.年龄 == mg.notin(10, 30, 45)          | 若字段值不是传入值的成员，则符合     |
 | mc.爱好 == mg.containAll('画画', '足球') | 若字段值包含传入值的所有元素，则符合 |
 | ...                                      | ...                                  |
 
-过滤器的集合运算：
+#### 过滤器的集合运算
 
-| **代码**                                                         | **解释** |
-| ---------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
-| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
-| [ ~(mc.年龄>100) ]                                                     | 补集           |
+| **代码**                                                       | **解释** |
+| -------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                         | 交集           |
+| [ (mc.年龄<30)\| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                      | 差集           |
+| [ ~(mc.年龄>100) ]                                                   | 补集           |
+
+#### 限定字段
 
 只返回姓名、年龄这2个字段：
 
 ```python
 await sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
-特殊操作：
+#### 特殊操作
 
 | 代码             | 解释                                               |
 | ---------------- | -------------------------------------------------- |
 | mup.inc(1)       | 自增1                                              |
 | mup.inc(-1)      | 自减1                                              |
 | mup.add(1, 2, 3) | 向列表字段添加元素，仅当被添加的元素不存在时才添加 |
 | ...              | ...                                                |
 
 # 支持作者1元
 
 asymongo 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `asymongo-1.3.2/pyproject.toml` & `asymongo-1.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymongo"
-version = "1.3.2"
+version = "1.3.3"
 description = "异步的 MongoDB ORM"
-dependencies = ["lccpy >=1.3.1"]
-keywords = ["asymongo", "motor", "mongodb", "pymongo"]
+dependencies = ["lccpy >=1.4.7"]
+keywords = ["asymongo", "motor", "mongodb", "pymongo", "orm"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `asymongo-1.3.2/PKG-INFO` & `asymongo-1.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,161 @@
 Metadata-Version: 2.1
 Name: asymongo
-Version: 1.3.2
+Version: 1.3.3
 Summary: 异步的 MongoDB ORM
-Keywords: asymongo,motor,mongodb,pymongo
+Keywords: asymongo,motor,mongodb,pymongo,orm
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.3.1
+Requires-Dist: lccpy >=1.4.7
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/asymongo#readme
 
 # 项目描述
 
 异步的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install asymongo`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/docs/doc.md)
 
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
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
 import asymongo as mg
 from asymongo import mc, mup
 ```
 
-创建ORM：
+#### 创建ORM
 
 ```python
 mkconn = lambda: MongoClient(host='localhost', port=27017)
 
 orm = mg.ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
-新增数据：
+#### 新增数据
 
 ```python
 line1 = {'姓名': '小一', '年龄':11, '幸运数字':[1, 2, 3], '成绩':{'语文':81, '数学':82}}
 line2 = {'姓名': '小二', '年龄':12, '幸运数字':[2, 3, 4], '成绩':{'语文':82, '数学':83}}
 line3 = {'姓名': '小三', '年龄':13, '幸运数字':[3, 4, 5], '成绩':{'语文':83, '数学':84}}
 line4 = {'姓名': '小四', '年龄':14, '幸运数字':[4, 5, 6], '成绩':{'语文':84, '数学':85}}
 line5 = {'姓名': '小五', '年龄':15, '幸运数字':[5, 6, 7], '成绩':{'语文':85, '数学':86}}
 line6 = {'姓名': '小六', '年龄':16, '幸运数字':[6, 7, 8], '成绩':{'语文':86, '数学':87}}
 
 await sheet.insert(line1)  # 添加1条数据
 await sheet.insert([ line2, line3, line4, line5, line6 ])  # 批量添加
 ```
 
-查询：
+#### 查询
 
 ```python
 await sheet[:]  # 查询所有数据
 
 await sheet[3]  # 查询第3条数据
 
 await sheet[mc.成绩.语文 == 85][:]  # 查询语文成绩为85分的数据
 
 await sheet[mc.年龄>13][mc.姓名=='小五'][1]  # 查询年龄大于13、且姓名叫'小五'的第1条数据
 ```
 
-修改：
+#### 修改
 
 ```python
 data = {
     '视力': 5.0,
     '性别': '男',
     '爱好': ['足球','篮球','画画','跳绳'],
     '幸运数字': mup.push(15,16,17),  # 添加到列表
     '年龄': mup.inc(2)  # 自增
 }
 
 await sheet.update(data)[2:5]
 ```
 
-删除：
+#### 删除
 
 ```python
 # 删除年龄>=15的数据
 await sheet[mc.年龄>=15].delete()[:]
 
 # 删除年龄大于10、且姓名包含'小'的第2条数据
 await sheet[mc.年龄>10][mc.姓名 == mg.re('小')].delete()[2]
 
 # 删除所有数据
 await sheet.delete()[:]
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
 
 | **代码**                           | **解释**                       |
 | ---------------------------------------- | ------------------------------------ |
 | mc.年级 == mg.isin('初三', '高二')       | 若字段值是传入值的成员，则符合       |
 | mc.年龄 == mg.notin(10, 30, 45)          | 若字段值不是传入值的成员，则符合     |
 | mc.爱好 == mg.containAll('画画', '足球') | 若字段值包含传入值的所有元素，则符合 |
 | ...                                      | ...                                  |
 
-过滤器的集合运算：
+#### 过滤器的集合运算
 
-| **代码**                                                         | **解释** |
-| ---------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
-| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
-| [ ~(mc.年龄>100) ]                                                     | 补集           |
+| **代码**                                                       | **解释** |
+| -------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                         | 交集           |
+| [ (mc.年龄<30)\| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                      | 差集           |
+| [ ~(mc.年龄>100) ]                                                   | 补集           |
+
+#### 限定字段
 
 只返回姓名、年龄这2个字段：
 
 ```python
 await sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
-特殊操作：
+#### 特殊操作
 
 | 代码             | 解释                                               |
 | ---------------- | -------------------------------------------------- |
 | mup.inc(1)       | 自增1                                              |
 | mup.inc(-1)      | 自减1                                              |
 | mup.add(1, 2, 3) | 向列表字段添加元素，仅当被添加的元素不存在时才添加 |
 | ...              | ...                                                |
 
 # 支持作者1元
 
 asymongo 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

