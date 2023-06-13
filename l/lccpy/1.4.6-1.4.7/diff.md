# Comparing `tmp/lccpy-1.4.6.tar.gz` & `tmp/lccpy-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lccpy-1.4.6.tar", last modified: Fri Jun  2 15:20:18 2023, max compression
+gzip compressed data, was "lccpy-1.4.7.tar", last modified: Tue Jun 13 15:41:03 2023, max compression
```

## Comparing `lccpy-1.4.6.tar` & `lccpy-1.4.7.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.6/LICENSE
--rw-r--r--   0        0        0      114 2023-04-30 19:30:52.062289 lccpy-1.4.6/README.md
--rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.6/lccpy/__init__.py
--rw-r--r--   0        0        0      143 2023-04-11 02:41:01.880058 lccpy-1.4.6/lccpy/_mtype.py
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.6/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
--rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.4.6/lccpy/asymongo/__init__.py
--rw-r--r--   0        0        0    20512 2023-04-11 02:42:19.557384 lccpy-1.4.6/lccpy/asymongo/_asymongo.py
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.6/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
--rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.4.6/lccpy/asymysql/__init__.py
--rw-r--r--   0        0        0    22806 2023-04-19 04:50:36.901729 lccpy-1.4.6/lccpy/asymysql/_asymysql.py
--rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.6/lccpy/coolfunc/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.6/lccpy/coolfunc/_coolfunc.py
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.6/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
--rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.4.6/lccpy/coolmongo/__init__.py
--rw-r--r--   0        0        0    20930 2023-04-11 02:42:37.661736 lccpy-1.4.6/lccpy/coolmongo/_coolmongo.py
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.6/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
--rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.4.6/lccpy/coolmysql/__init__.py
--rw-r--r--   0        0        0    22832 2023-04-19 07:49:15.385992 lccpy-1.4.6/lccpy/coolmysql/_coolmysql.py
--rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.6/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
--rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.4.6/lccpy/encrypt256/__init__.py
--rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.6/lccpy/encrypt256/_encrypt256.py
--rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.4.6/lccpy/increment/__init__.py
--rw-r--r--   0        0        0     1586 2023-06-02 08:06:48.314577 lccpy-1.4.6/lccpy/increment/_increment.py
--rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.6/lccpy/rstyleslice/__init__.py
--rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.6/lccpy/rstyleslice/_rstyleslice.py
--rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.4.6/lccpy/vtype/__init__.py
--rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.6/lccpy/vtype/_cooltime.py
--rw-r--r--   0        0        0    11771 2023-04-12 12:56:02.300717 lccpy-1.4.6/lccpy/vtype/_vtype.py
--rw-r--r--   0        0        0      565 2023-06-02 15:18:23.324861 lccpy-1.4.6/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 lccpy-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.7/LICENSE
+-rw-r--r--   0        0        0      112 2023-06-13 05:52:50.378292 lccpy-1.4.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.7/lccpy/__init__.py
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.7/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
+-rw-r--r--   0        0        0      165 2023-06-13 11:57:21.300071 lccpy-1.4.7/lccpy/asymongo/__init__.py
+-rw-r--r--   0        0        0    20497 2023-06-13 11:57:21.300071 lccpy-1.4.7/lccpy/asymongo/_core.py
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.7/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
+-rw-r--r--   0        0        0       86 2023-06-13 11:57:21.290462 lccpy-1.4.7/lccpy/asymysql/__init__.py
+-rw-r--r--   0        0        0    22791 2023-06-13 11:57:21.299172 lccpy-1.4.7/lccpy/asymysql/_core.py
+-rw-r--r--   0        0        0    11358 2023-05-14 02:53:10.000000 lccpy-1.4.7/lccpy/coolapi/Licenses of dependent packages/tornado/LICENSE
+-rw-r--r--   0        0        0       40 2023-05-28 06:10:27.855895 lccpy-1.4.7/lccpy/coolapi/__init__.py
+-rw-r--r--   0        0        0     1668 2023-05-27 11:00:33.037396 lccpy-1.4.7/lccpy/coolapi/_core.py
+-rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.7/lccpy/coolfunc/__init__.py
+-rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.7/lccpy/coolfunc/_coolfunc.py
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.7/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      165 2023-06-13 11:57:21.279654 lccpy-1.4.7/lccpy/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20915 2023-06-13 11:57:21.290462 lccpy-1.4.7/lccpy/coolmongo/_core.py
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.7/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       86 2023-06-13 11:57:21.279654 lccpy-1.4.7/lccpy/coolmysql/__init__.py
+-rw-r--r--   0        0        0    22817 2023-06-13 11:57:21.279654 lccpy-1.4.7/lccpy/coolmysql/_core.py
+-rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.7/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
+-rw-r--r--   0        0        0       29 2023-06-13 11:40:05.743411 lccpy-1.4.7/lccpy/encrypt256/__init__.py
+-rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.7/lccpy/encrypt256/_core.py
+-rw-r--r--   0        0        0       30 2023-06-13 11:40:37.720315 lccpy-1.4.7/lccpy/increment/__init__.py
+-rw-r--r--   0        0        0     1586 2023-06-02 08:06:48.314577 lccpy-1.4.7/lccpy/increment/_core.py
+-rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.7/lccpy/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.7/lccpy/rstyleslice/_rstyleslice.py
+-rw-r--r--   0        0        0      179 2023-06-13 12:23:13.409389 lccpy-1.4.7/lccpy/vtype/__init__.py
+-rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.7/lccpy/vtype/_cooltime.py
+-rw-r--r--   0        0        0    10266 2023-06-13 14:45:35.809939 lccpy-1.4.7/lccpy/vtype/_vtype.py
+-rw-r--r--   0        0        0      574 2023-06-13 15:36:41.801055 lccpy-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 lccpy-1.4.7/PKG-INFO
```

### Comparing `lccpy-1.4.6/LICENSE` & `lccpy-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE` & `lccpy-1.4.7/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/asymongo/_asymongo.py` & `lccpy-1.4.7/lccpy/asymongo/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 license: Apache License, Version 2.0
 email: lcctoor@outlook.com
 '''
 
 from copy import deepcopy
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient  # 代码提示
 
-from ..vtype import uniset, empset, SysEmpty, ToolPool
-from .._mtype import MgIndexError
+from ..vtype import uniset, empset, SysEmpty, ToolPool, OrmIndexError
 
 
 class Factory:
     _variable = True
 
     def __init__(self, where):
         if where is not empset:
@@ -277,15 +276,15 @@
             r = await sheet.delete_one(ParseWhere(self))
             self.connPool.put(conn)
             return r
             # r.acknowledged, r.deleted_count
         # 其它情况
         try:
             ids = await self['_id'][key]
-        except MgIndexError:
+        except OrmIndexError:
             condition = Factory(empset).ParseWhere()
             r = await sheet.delete_one(condition)
             self.connPool.put(conn)
             return r
         else:
             if isinstance(ids, list):
                 condition = (mc._id == isin(*ids)).ParseWhere()
@@ -333,15 +332,15 @@
                 r = await sheet.update_one(empsetCondi, {'$setOnInsert':default}, upsert=True)
             self.connPool.put(conn)
             return r
             # r.acknowledged, r.matched_count
         # 其它情况
         try:
             ids = await self['_id'][key]
-        except MgIndexError:
+        except OrmIndexError:
             if repairUpsert and default:
                 r = await sheet.update_one(empsetCondi, {'$setOnInsert':default}, upsert=True)
             else:
                 r = await sheet.update_one(empsetCondi, {'$set':{}})
             self.connPool.put(conn)
             return r
         else:
@@ -377,29 +376,29 @@
             return self[index]
         except IndexError:
             return default
 
     async def _find_one(self, key):
         index = key
         if index < 0: index = await self.len() + index + 1
-        if index < 1: raise MgIndexError(f"index({key}) out of range")
+        if index < 1: raise OrmIndexError(f"index({key}) out of range")
         skip = index - 1
         conn:MongoClient = self.connPool.get()
         sheet = conn[self.dbName][self.sheetName]
         sh = sheet.find(ParseWhere(self), self._ParseColumns())
         if sort:= self._ParseOrder():
             sh = sh.sort(sort)
         if skip: sh = sh.skip(skip)
         r = await sh.limit(1).to_list(1)
         self.connPool.put(conn)
         if r:
             return r[0]
         else:
-            raise MgIndexError(f"index({key}) out of range")
-            # 没有的话引发MgIndexError错误. 已被self.update和self.delete调用
+            raise OrmIndexError(f"index({key}) out of range")
+            # 没有的话引发OrmIndexError错误. 已被self.update和self.delete调用
 
     async def _find_many(self, key):
         # 没有的话返回空列表, 但不要报错. 已被self.update和self.delete调用
         L, R, S = key.start, key.stop, key.step or 1
         tL, tR, tS = type(L), type(R), type(S)
         assert {tL, tR, tS} <= {int, type(None)}
         assert 0 not in (L, R)
```

### Comparing `lccpy-1.4.6/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE` & `lccpy-1.4.7/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/asymysql/_asymysql.py` & `lccpy-1.4.7/lccpy/asymysql/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 email: lcctoor@outlook.com
 '''
 
 from copy import deepcopy
 from collections import deque
 from aiomysql.cursors import DictCursor
 
-from ..vtype import uniset, empset, SysEmpty
+from ..vtype import uniset, empset, SysEmpty, OrmIndexError
 from ..coolfunc import jsonChinese
-from .._mtype import MgIndexError
 
 
 class ToolPool():
     async def asy_init(self, mktool, minlen:int=0, maxlen=None):
         self.mktool = mktool
         self.pool = deque([await mktool() for i in range(minlen or 0)], maxlen=maxlen)
     
@@ -389,15 +388,15 @@
         if key == 1 and not self._ParseOrder():
             rdata, cursor = await self.execute(f"delete from {self.sheetName}{self.where} limit 1")
             return cursor
         # 其它情况
         pk = await self.getPK()
         try:
             pks = await self[pk][key]
-        except MgIndexError:
+        except OrmIndexError:
             rdata, cursor = await self.execute(f"delete from {self.sheetName} where 1 = 2 limit 1")
         else:
             if isinstance(pks, list):
                 if pks:
                     pks = [x[pk] for x in pks]
                     rdata, cursor = await self.execute(f"delete from {self.sheetName}{mc[pk].isin(*pks)}")
                 else:
@@ -422,15 +421,15 @@
         if key == 1 and not self._ParseOrder():
             rdata, cursor = await self.execute(f"update {self.sheetName} set {data}{self.where} limit 1")
             return cursor
         # 其它情况
         pk = await self.getPK()
         try:
             pks = await self[pk][key]
-        except MgIndexError:
+        except OrmIndexError:
             rdata, cursor = await self.execute(f"update {self.sheetName} set {data} where 1 = 2 limit 1")
         else:
             if isinstance(pks, list):
                 if pks:
                     pks = [x[pk] for x in pks]
                     rdata, cursor = await self.execute(f"update {self.sheetName} set {data}{mc[pk].isin(*pks)}")
                 else:
@@ -503,24 +502,24 @@
             self._updateBase(key, data=value)
         else:
             raise TypeError(key)
         
     async def _find_one(self, key):
         index = key
         if index < 0: index = await self.len() + index + 1  # R索引
-        if index < 1: raise MgIndexError(f"index({key}) out of range")
+        if index < 1: raise OrmIndexError(f"index({key}) out of range")
         skip = index - 1
         parseLimit = f" limit {skip}, 1"
         sql = f"select {self._ParseColumns()} from {self.sheetName}{self.where}{self._ParseOrder()}{parseLimit}"
         r, cursor = await self.execute(sql, commit=False)
         if r:
             return r[0]
         else:
-            raise MgIndexError(f"index({key}) out of range")
-            # 没有的话引发MgIndexError错误. 已被self.update和self.delete调用
+            raise OrmIndexError(f"index({key}) out of range")
+            # 没有的话引发OrmIndexError错误. 已被self.update和self.delete调用
 
     async def _find_many(self, key):
         # 没有的话返回空列表, 但不要报错. 已被self.update和self.delete调用
         L, R, S = key.start, key.stop, key.step or 1
         tL, tR, tS = type(L), type(R), type(S)
         assert {tL, tR, tS} <= {int, type(None)}
         assert 0 not in (L, R)
```

### Comparing `lccpy-1.4.6/lccpy/coolfunc/_coolfunc.py` & `lccpy-1.4.7/lccpy/coolfunc/_coolfunc.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE` & `lccpy-1.4.7/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/coolmongo/_coolmongo.py` & `lccpy-1.4.7/lccpy/coolmongo/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 license: Apache License, Version 2.0
 email: lcctoor@outlook.com
 '''
 
 from copy import deepcopy
 from pymongo import MongoClient  # 代码提示
 
-from ..vtype import uniset, empset, SysEmpty, ToolPool
-from .._mtype import MgIndexError
+from ..vtype import uniset, empset, SysEmpty, ToolPool, OrmIndexError
 
 
 class Factory:
     _variable = True
 
     def __init__(self, where):
         if where is not empset:
@@ -274,15 +273,15 @@
             r = sheet.delete_one(ParseWhere(self))
             self.connPool.put(conn)
             return r
             # r.acknowledged, r.deleted_count
         # 其它情况
         try:
             ids = self['_id'][key]
-        except MgIndexError:
+        except OrmIndexError:
             condition = Factory(empset).ParseWhere()
             r = sheet.delete_one(condition)
             self.connPool.put(conn)
             return r
         else:
             if isinstance(ids, list):
                 condition = (mc._id == isin(*ids)).ParseWhere()
@@ -330,15 +329,15 @@
                 r = sheet.update_one(empsetCondi, {'$setOnInsert':default}, upsert=True)
             self.connPool.put(conn)
             return r
             # r.acknowledged, r.matched_count
         # 其它情况
         try:
             ids = self['_id'][key]
-        except MgIndexError:
+        except OrmIndexError:
             if repairUpsert and default:
                 r = sheet.update_one(empsetCondi, {'$setOnInsert':default}, upsert=True)
             else:
                 r = sheet.update_one(empsetCondi, {'$set':{}})
             self.connPool.put(conn)
             return r
         else:
@@ -384,29 +383,29 @@
             raise TypeError(key)
     
     def __getitem__(self, key):
         # 索引取值
         if isinstance(key, int):
             index = key
             if index < 0: index = len(self) + index + 1
-            if index < 1: raise MgIndexError(f"index({key}) out of range")
+            if index < 1: raise OrmIndexError(f"index({key}) out of range")
             skip = index - 1
             conn:MongoClient = self.connPool.get()
             sheet = conn[self.dbName][self.sheetName]
             sh = sheet.find(ParseWhere(self), self._ParseColumns())
             if sort:= self._ParseOrder():
                 sh = sh.sort(sort)
             if skip: sh = sh.skip(skip)
             r = list(sh.limit(1))
             self.connPool.put(conn)
             if r:
                 return r[0]
             else:
-                raise MgIndexError(f"index({key}) out of range")
-                # 没有的话引发MgIndexError错误. 已被self.update和self.delete调用
+                raise OrmIndexError(f"index({key}) out of range")
+                # 没有的话引发OrmIndexError错误. 已被self.update和self.delete调用
         # 切片取值
         if isinstance(key, slice):
             # 没有的话返回空列表, 但不要报错. 已被self.update和self.delete调用
             L, R, S = key.start, key.stop, key.step or 1
             tL, tR, tS = type(L), type(R), type(S)
             assert {tL, tR, tS} <= {int, type(None)}
             assert 0 not in (L, R)
```

### Comparing `lccpy-1.4.6/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE` & `lccpy-1.4.7/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/coolmysql/_coolmysql.py` & `lccpy-1.4.7/lccpy/coolmysql/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 '''
 
 from copy import deepcopy
 from collections import deque
 from pymysql import connect  # 代码提示
 from pymysql.cursors import DictCursor
 
-from ..vtype import uniset, empset, SysEmpty
+from ..vtype import uniset, empset, SysEmpty, OrmIndexError
 from ..coolfunc import jsonChinese
-from .._mtype import MgIndexError
 
 
 class ToolPool():
     def __init__(self, mktool, minlen:int=0, maxlen=None):
         self.mktool = mktool
         self.pool = deque([mktool() for i in range(minlen or 0)], maxlen=maxlen)
     
@@ -387,15 +386,15 @@
         if key == 1 and not self._ParseOrder():
             rdata, cursor = self.execute(f"delete from {self.sheetName}{self.where} limit 1")
             return cursor
         # 其它情况
         pk = self.getPK()
         try:
             pks = self[pk][key]
-        except MgIndexError:
+        except OrmIndexError:
             rdata, cursor = self.execute(f"delete from {self.sheetName} where 1 = 2 limit 1")
         else:
             if isinstance(pks, list):
                 if pks:
                     pks = [x[pk] for x in pks]
                     rdata, cursor = self.execute(f"delete from {self.sheetName}{mc[pk].isin(*pks)}")
                 else:
@@ -420,15 +419,15 @@
         if key == 1 and not self._ParseOrder():
             rdata, cursor = self.execute(f"update {self.sheetName} set {data}{self.where} limit 1")
             return cursor
         # 其它情况
         pk = self.getPK()
         try:
             pks = self[pk][key]
-        except MgIndexError:
+        except OrmIndexError:
             rdata, cursor = self.execute(f"update {self.sheetName} set {data} where 1 = 2 limit 1")
         else:
             if isinstance(pks, list):
                 if pks:
                     pks = [x[pk] for x in pks]
                     rdata, cursor = self.execute(f"update {self.sheetName} set {data}{mc[pk].isin(*pks)}")
                 else:
@@ -504,24 +503,24 @@
             raise TypeError(key)
     
     def __getitem__(self, key):
         # 索引取值
         if isinstance(key, int):
             index = key
             if index < 0: index = len(self) + index + 1  # R索引
-            if index < 1: raise MgIndexError(f"index({key}) out of range")
+            if index < 1: raise OrmIndexError(f"index({key}) out of range")
             skip = index - 1
             parseLimit = f" limit {skip}, 1"
             sql = f"select {self._ParseColumns()} from {self.sheetName}{self.where}{self._ParseOrder()}{parseLimit}"
             r, cursor = self.execute(sql, commit=False)
             if r:
                 return r[0]
             else:
-                raise MgIndexError(f"index({key}) out of range")
-                # 没有的话引发MgIndexError错误. 已被self.update和self.delete调用
+                raise OrmIndexError(f"index({key}) out of range")
+                # 没有的话引发OrmIndexError错误. 已被self.update和self.delete调用
         # 切片取值
         if isinstance(key, slice):
             # 没有的话返回空列表, 但不要报错. 已被self.update和self.delete调用
             L, R, S = key.start, key.stop, key.step or 1
             tL, tR, tS = type(L), type(R), type(S)
             assert {tL, tR, tS} <= {int, type(None)}
             assert 0 not in (L, R)
```

### Comparing `lccpy-1.4.6/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE` & `lccpy-1.4.7/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/encrypt256/_encrypt256.py` & `lccpy-1.4.7/lccpy/encrypt256/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/increment/_increment.py` & `lccpy-1.4.7/lccpy/increment/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/rstyleslice/_rstyleslice.py` & `lccpy-1.4.7/lccpy/rstyleslice/_rstyleslice.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/vtype/_cooltime.py` & `lccpy-1.4.7/lccpy/vtype/_cooltime.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.6/lccpy/vtype/_vtype.py` & `lccpy-1.4.7/lccpy/vtype/_vtype.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 import re
 from decimal import Decimal
 from math import ceil
 from collections import deque
 import hashlib
 from hashlib import shake_256
 from fractions import Fraction
-from typing import Union
+from typing import Union, Any
+
+
+class missing_arguments_error(Exception): ...
 
 
 ########################################## vbool ##########################################
 
 class vbool():
-    '''
-        解决 1 == True 的历史遗留问题
-    '''
+    ''' 解决 1 == True 的历史遗留问题 '''
+    
     name: str
+    core: bool
     _hash_value: int
-    _bool_vlaue: bool
+    
     def __new__(cls, value, name='', _sysValue=False):
         if _sysValue:
             self = object.__new__(cls)
             self.name = name
-            self._bool_vlaue = bool(value)
+            self.core = bool(value)
             return self
         else:
             return vtrue if value else vfalse
 
-    def __bool__(self): return self._bool_vlaue
+    def __bool__(self): return self.core
     def __eq__(self, o): return self is o
     def __str__(self): return self.name
 
 vtrue = vbool(True, 'vtrue', _sysValue=True)
 vfalse = vbool(False, 'vfalse', _sysValue=True)
 
 uniset = vbool(True, 'uniset', _sysValue=True)  # 全集
@@ -44,15 +47,15 @@
 
 SysEmpty = vbool(False, 'SysEmpty', _sysValue=True)
     # 供开发者调用的表示空的标识, 如:
         # 作为默认参数以识别调用者是否传参
         # 在函数内部作为某种状态标识
     # 此参数只允许函数开发者引用, 禁止函数调用者引用.
 
-########################################## bidict ##########################################
+##################################################################################
 
 class bidict:
     ''' 双向字典 '''
     def __init__(self):
         self.core = {}
     
     def __setitem__(self, key, value):
@@ -63,270 +66,227 @@
     
     def __getitem__(self, key):
         return self.core[key]
 
     def get(self, key, default=SysEmpty):
         value = self.core.get(key, default)
         if value is SysEmpty:
-            {}.get(key)
-        return value
+            raise missing_arguments_error('default')
+        else:
+            return value
     
     def pop(self, key, default=SysEmpty):
         if key in self.core:
             value = self.core.pop(key)
-            self.core.pop(value)
+            self.core.pop(value, 0)
             return value
         elif default is SysEmpty:
-            {}.pop(key)
+            raise missing_arguments_error('default')
         else:
             return default
 
-########################################## ztype ##########################################
-
-class WillCover:
-    '''
-    如果父类中的某个变量等于此类, 则表示该变量必须在子类中被覆盖.
-    '''
-    def __init__(self, *vs, **kvs):
-        raise Exception('WillCover')
+##################################################################################
 
 
 class ztype():
-    core: Union[int, float, str, tuple, list, set, dict, Fraction]
-    selfType = WillCover
+    core: Any
 
     def __getattr__(self, name):
         return self.core.__getattr__(name)
     
     @classmethod
-    def _ztypeCore(cls, obj):
+    def _GetCore(cls, obj):
         if isinstance(obj, ztype):
             return obj.core
         return obj
     
-    @classmethod
-    def _sonTypeCore(cls, obj):
-        if isinstance(obj, cls):  # cls的值会随着子类而变化
-            return obj.core
-        return obj
-    
     def __str__(self): return str(self.core)
     def __int__(self): return int(self.core)
     def __float__(self): return float(self.core)
     def __bool__(self): return bool(self.core)
+    def __bytes__(self): return bytes(self.core)
+
     def str(self): return str(self)
     def int(self): return int(self)
     def float(self): return float(self)
     def bool(self): return bool(self)
-    def vbool(self): return vbool(self)
+    def bytes(self): return bytes(self.core)
 
-    def __iter__(self): yield from self.core
     def __len__(self): return len(self.core)
 
     # 默认用内核比较大小
-    def __eq__(self, obj): return self.core == self._ztypeCore(obj)
-    def __ne__(self, obj): return self.core != self._ztypeCore(obj)
-    def __lt__(self, obj): return self.core < self._ztypeCore(obj)
-    def __le__(self, obj): return self.core <= self._ztypeCore(obj)
-    def __gt__(self, obj): return self.core > self._ztypeCore(obj)
-    def __ge__(self, obj): return self.core >= self._ztypeCore(obj)
+    def __eq__(self, obj): return self.core == self._GetCore(obj)
+    def __ne__(self, obj): return self.core != self._GetCore(obj)
+    def __lt__(self, obj): return self.core < self._GetCore(obj)
+    def __le__(self, obj): return self.core <= self._GetCore(obj)
+    def __gt__(self, obj): return self.core > self._GetCore(obj)
+    def __ge__(self, obj): return self.core >= self._GetCore(obj)
 
     # 加减乘除默认用内核操作
-    def __mul__(self, n): return self.selfType(self.core * self._ztypeCore(n), SysEmpty)
-    def __rmul__(self, n): return self.selfType(self.core * self._ztypeCore(n), SysEmpty)
-    def __add__(self, n): return self.selfType(self.core + self._ztypeCore(n), SysEmpty)
-    def __radd__(self, n): return self.selfType(self.core + self._ztypeCore(n), SysEmpty)
-    def __sub__(self, n): return self.selfType(self.core - self._ztypeCore(n), SysEmpty)
-    def __rsub__(self, n): return self.selfType(self._ztypeCore(n) - self.core, SysEmpty)
-    def __truediv__(self, n): return self.selfType(self.core / self._ztypeCore(n), SysEmpty)
-    def __rtruediv__(self, n): return self.selfType(self._ztypeCore(n) / self.core, SysEmpty)
+    def __add__(self, n): return self.__class__(self.core + self._GetCore(n))
+    def __radd__(self, n): return self.__class__(self._GetCore(n) + self.core)
     def __iadd__(self, n):
-        self.core += self._ztypeCore(n)
+        self.core += self._GetCore(n)
         return self
+    
+    def __sub__(self, n): return self.__class__(self.core - self._GetCore(n))
+    def __rsub__(self, n): return self.__class__(self._GetCore(n) - self.core)
     def __isub__(self, n):
-        self.core -= self._ztypeCore(n)
+        self.core -= self._GetCore(n)
         return self.core
+
+    def __mul__(self, n): return self.__class__(self.core * self._GetCore(n))
+    def __rmul__(self, n): return self.__class__(self._GetCore(n) * self.core)
     def __imul__(self, n):
-        self.core *= self._ztypeCore(n)
+        self.core *= self._GetCore(n)
         return self
+
+    def __truediv__(self, n): return self.__class__(self.core / self._GetCore(n))
+    def __rtruediv__(self, n): return self.__class__(self._GetCore(n) / self.core)
     def __itruediv__(self, n):
-        self.core /= self._ztypeCore(n)
+        self.core /= self._GetCore(n)
         return self
 
 
-########################################## vnum ##########################################
-
-class vnum(ztype):
-    '''
-        1. float和int没必要拆成两种, 太麻烦了
-        2. 解决浮点数精度问题
-    '''
-    def __new__(cls, numerator, denominator=SysEmpty):
-        self = object.__new__(cls)
-        self.selfType = cls
-        # 创建core
-        numerator = self._intoFraction(numerator)
-        if denominator is SysEmpty:
-            self.core = numerator
-        else:
-            self.core = Fraction(numerator, self._intoFraction(denominator))
-        return self
-
-    @classmethod
-    def _intoFraction(cls, v):
-        try:
-            v = v._vnum_()  # _vnum_为预处理方法, 它将v处理成本方法能够处理的数据.
-        except:
-            pass
-        if isinstance(v, (int, float)): return Fraction(v)
-        if isinstance(v, Fraction): return v
-        if isinstance(v, cls): return v.core
-        if isinstance(v, str): return Fraction(Decimal(v))
-        if v in (None,): return Fraction(0)
-        raise TypeError(type(v))
+##################################################################################
 
-    def __hash__(self): return hash(self.core)  # 使用内核的哈希值作为字典的键
+class vbytes(ztype):
+    ''' 可变字节串 '''
 
+    core: bytes
 
-########################################## vdict ##########################################
+    def __bytes__(self): return self.core
+    def __init__(self, *s, **kvs):
+        self.core = bytes(*s, **kvs)
 
-def _XpathGet(dic, i, keySize, keys):
-    if i < keySize and type(dic) is dict:
-        ikey = keys[i]
-        for k, v in dic.items():
-            if k == ikey:
-                if i == keySize - 1:
-                    return v
-                value = _XpathGet(v, i + 1, keySize, keys)
-                if value is not SysEmpty:
-                    return value
-            else:
-                value = _XpathGet(v, i, keySize, keys)
-                if value is not SysEmpty:
-                    return value
-    return SysEmpty
+    def md5(self, rtype:str='str'):
+        value = hashlib.md5(self.core)
+        if rtype in (str, 'str'): return value.hexdigest()
+        if rtype in (bytes, 'bytes'): return value.digest()
+        if rtype in (vbytes, 'vbytes'): return vbytes(value.digest())
+        raise ValueError(rtype)
 
+    def shake256(self, rtype:str='str', rsize=32):
+        value = shake_256(self.core)
+        if rtype in (str, 'str'): return value.hexdigest(ceil(rsize/2))[:rsize]
+        if rtype in (bytes, 'bytes'): return value.digest(rsize)
+        if rtype in (vbytes, 'vbytes'): return vbytes(value.digest(rsize))
+        raise ValueError(rtype)
 
-class vdict(ztype):
-    def __new__(cls, obj=SysEmpty, **kvs):
-        self = object.__new__(cls)
-        self.selfType = cls
-        # 创建core
-        if obj is SysEmpty:
-            self.core = kvs
-        else:
-            try:
-                self.core = dict(obj)
-            except:
-                try:
-                    self.core = dict(obj._dict_())
-                except:
-                    if obj in (None,):
-                        self.core = {}
-                    else:
-                        raise ValueError(obj)
-        return self
-
-    def xpath(self, *keys):
-        '''
-            一个查找字典的子孙键的工具.
-            使用场景: 当字典的结构具有不确定性, 或者要获取的键位于较深层的子孙层时, 可使用该函数进行取值.
-        '''
-        if not isinstance(keys, tuple):
-            keys = (keys, )
-        value = _XpathGet(self.core, 0, len(keys), keys)
-        if value is SysEmpty:
-            raise KeyError(keys)
-        return value
-    
-    def deepGet(self, *keys, default=None):
-        res = self.core
-        try:
-            for k in keys:
-                res = res[k]
-            return res
-        except:
-            return default
-
-########################################## vstr ##########################################
+##################################################################################
 
 class vstr(ztype):
+    ''' 可变字符串 '''
+
+    core: str
 
     s_a = 'abcdefghijklmnopqrstuvwxyz'
     s_A = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
     s_0 = '0123456789'
     s_0a = '0123456789abcdefghijklmnopqrstuvwxyz'
     s_0A = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ'
     s_aA = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
     s_0aA = '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
 
-    def __new__(cls, obj=SysEmpty, **kvs):
-        self = object.__new__(cls)
-        self.selfType = cls
-        self.core = str(obj)
-        return self
+    def __str__(self): return self.core
+    def __init__(self, *s, **kvs):
+        self.core = str(*s, **kvs)
 
     def wash_paragraph(self):  # 单段清洗
         text = re.sub('\s+', ' ', self.core)
         text = re.sub('^ +', '', text)
         text = re.sub(' +$', '', text)
         return vstr(text)
 
     def sub(self, pattern, repl, count=0, flags=0):
         return vstr(re.sub(pattern, repl, self.core, count, flags))
 
     def visible(self):  # 是否含可视字符
-        return vbool(re.search('[^\s]', self.core))
+        return bool(re.search('[^\s]', self.core))
 
     def has_sound(self):   # 是否含有有声字符(支持中文和英文)
-        return vbool(re.search('[\u4e00-\u9fa5\da-zA-Z]', self.core))
+        return bool(re.search('[\u4e00-\u9fa5\da-zA-Z]', self.core))
 
     def has_chinese(self):
-        return vbool(re.search('[\u4e00-\u9fa5]', self.core))
+        return bool(re.search('[\u4e00-\u9fa5]', self.core))
 
-    def __bytes__(self): return self.core.encode('utf8')
+    def __contains__(self, obj):
+        if isinstance(obj, self.__class__):
+            return obj.core in self.core
+        return obj in self.core
+
+#################################################################################
+def into_Fraction(*s, **kvs):
+    if s and isinstance(s[0], vnum): return s[0].core
+    return Fraction(*s, **kvs)
 
-    def md5(self, rtype=str):
-        value = hashlib.md5(bytes(self))
-        if rtype in (str, 'str'): return value.hexdigest()
-        if rtype in (bytes, 'bytes'): return value.digest()
-        if rtype in (vstr, 'vstr'): return vstr(value.hexdigest())
-        raise TypeError(rtype)
+class vnum(ztype):
+    ''' 可变数字
+        1、 float 和 int 没必要拆成两种, 太麻烦了
+        2、 解决浮点数精度问题
+    '''
+    core: Fraction
+    
+    def __init__(self, numerator, denominator=SysEmpty):
+        if denominator is SysEmpty:
+            self.core = into_Fraction(numerator)
+        else:
+            self.core = Fraction(into_Fraction(numerator), into_Fraction(denominator))
 
-    def shake256(self, rtype='vstr', rsize=32):
-        value = shake_256(bytes(self))
-        if rtype is str: return value.hexdigest(ceil(rsize/2))[:rsize]
-        if rtype in ('vstr', vstr): return vstr(value.hexdigest(ceil(rsize/2))[:rsize])
-        if rtype is bytes: return value.digest(rsize)
-        raise TypeError(rtype)
+##################################################################################
 
-    def __hash__(self): return hash(self.core)  # 使用内核的哈希值作为字典的键
-    def __contains__(self, obj): return self._sonTypeCore(obj) in self.core
+def XpathGet(dic, i, keySize, keys):
+    if i < keySize and type(dic) is dict:
+        ikey = keys[i]
+        for k, v in dic.items():
+            if k == ikey:
+                if i == keySize - 1:
+                    return v
+                value = XpathGet(v, i + 1, keySize, keys)
+                if value is not SysEmpty:
+                    return value
+            else:
+                value = XpathGet(v, i, keySize, keys)
+                if value is not SysEmpty:
+                    return value
+    return SysEmpty
 
+def into_dict(*s, **kvs):
+    if s and isinstance(s[0], vdict): return s[0].core.copy()
+    return dict(*s, **kvs)
 
-########################################## vbytes ##########################################
+class vdict(ztype):
+    core: dict
 
-class vbytes(ztype):
+    def __init__(self, *s, **kvs):
+        self.core = into_dict(*s, **kvs)
 
-    def __new__(cls, obj=b''):
-        self = object.__new__(cls)
-        self.selfType = cls
+    def xpath(self, *keys):
+        '''
+            一个查找字典的子孙键的工具.
+            使用场景: 当字典的结构具有不确定性, 或者要获取的键位于较深层的子孙层时, 可使用该函数进行取值.
+        '''
+        if not isinstance(keys, tuple):
+            keys = (keys, )
+        value = XpathGet(self.core, 0, len(keys), keys)
+        if value is SysEmpty:
+            raise KeyError(keys)
+        return value
+    
+    def deepGet(self, *keys, default=SysEmpty):
+        res = self.core
         try:
-            self.core = bytes(obj)
+            for k in keys:
+                res = res[k]
+            return res
         except:
-            if isinstance(obj, str):
-                self.core = obj.encode('utf8')
-            elif isinstance(obj, (int, float)):
-                self.core = bytes([int(obj)])
-            elif obj in (None,):
-                self.core = b''
+            if default is SysEmpty:
+                raise missing_arguments_error('default')
             else:
-                raise
-        return self
-
+                return default
 
 ########################################## ToolPool ##########################################
 
 class ToolPool():
     def __init__(self, mktool, minlen:int=0, maxlen=None):
         self.mktool = mktool
         self.pool = deque([mktool() for i in range(minlen or 0)], maxlen=maxlen)
@@ -337,8 +297,14 @@
     def get(self):  # 左出
         try:
             return self.beforeGet(self.pool.popleft())
         except:
             return self.mktool()
     
     def beforeGet(self, obj): return obj
-    def beforePut(self, obj): return obj
+    def beforePut(self, obj): return obj
+
+
+class OrmIndexError(IndexError):
+    # 供 coolmysql、coolmongo、asymysql、asymongo 调用
+    def __repr__(self):
+        return 'OrmIndexError'
```

### Comparing `lccpy-1.4.6/pyproject.toml` & `lccpy-1.4.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lccpy"
-version = "1.4.6"
-description = "项目 <让 Python 更简单一点> 的依赖包"
-dependencies = ["motor", "aiomysql", "pymongo", "pymysql", "pycryptodome"]
+version = "1.4.7"
+description = "项目 <让Python更简单一点> 的依赖包"
+dependencies = ["motor", "aiomysql", "pymongo", "pymysql", "pycryptodome", "tornado"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `lccpy-1.4.6/PKG-INFO` & `lccpy-1.4.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: lccpy
-Version: 1.4.6
-Summary: 项目 <让 Python 更简单一点> 的依赖包
+Version: 1.4.7
+Summary: 项目 <让Python更简单一点> 的依赖包
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: motor
 Requires-Dist: aiomysql
 Requires-Dist: pymongo
 Requires-Dist: pymysql
 Requires-Dist: pycryptodome
+Requires-Dist: tornado
 Project-URL: HomePage, https://github.com/lcctoor/lccpy#readme
 
 # 项目描述
 
-项目 \<[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)\> 的依赖包。
+项目 \<[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)\> 的依赖包。
```

