# Comparing `tmp/nonebot_plugin_bottle-1.0.1.2.tar.gz` & `tmp/nonebot_plugin_bottle-1.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bottle-1.0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_bottle-1.0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_bottle-1.0.1.2.tar` & `nonebot_plugin_bottle-1.0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7814 2023-05-20 04:13:55.167748 nonebot_plugin_bottle-1.0.1.2/README.md
--rw-r--r--   0        0        0    20211 2023-05-20 04:13:55.167748 nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/__init__.py
--rw-r--r--   0        0        0      636 2023-05-20 04:13:55.167748 nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/config.py
--rw-r--r--   0        0        0    19027 2023-05-20 04:13:55.167748 nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/data_source.py
--rw-r--r--   0        0        0     2646 2023-05-20 04:13:55.167748 nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
--rw-r--r--   0        0        0     1426 2023-05-20 04:13:55.167748 nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/model.py
--rw-r--r--   0        0        0      968 2023-05-20 04:13:55.167748 nonebot_plugin_bottle-1.0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8577 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7814 2023-06-13 13:35:43.770040 nonebot_plugin_bottle-1.0.1.3/README.md
+-rw-r--r--   0        0        0    20345 2023-06-13 13:35:43.770040 nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/__init__.py
+-rw-r--r--   0        0        0      636 2023-06-13 13:35:43.770040 nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/config.py
+-rw-r--r--   0        0        0    19027 2023-06-13 13:35:43.770040 nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/data_source.py
+-rw-r--r--   0        0        0     2646 2023-06-13 13:35:43.770040 nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
+-rw-r--r--   0        0        0     1426 2023-06-13 13:35:43.770040 nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/model.py
+-rw-r--r--   0        0        0      965 2023-06-13 13:35:43.770040 nonebot_plugin_bottle-1.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8574 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_bottle-1.0.1.2/README.md` & `nonebot_plugin_bottle-1.0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/__init__.py` & `nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
     清空漂流瓶
     恢复漂流瓶 [漂流瓶编号]
     删除漂流瓶评论 [漂流瓶编号] [QQ号]
     漂流瓶白名单 [QQ / 群聊 / 举报] [QQ号 / 群号]
     漂流瓶黑名单 [QQ / 群聊] [QQ号 / 群号]
     漂流瓶详情 [漂流瓶编号]
 """.strip(),
+    type="application",
+    homepage="https://github.com/Todysheep/nonebot_plugin_bottle",
+    supported_adapters={"~onebot.v11"},
     extra={
         "unique_name": "nonebot_plugin_bottle",
         "example": "扔漂流瓶\n寄漂流瓶\n捡漂流瓶\n评论漂流瓶\n举报漂流瓶\n查看漂流瓶\n删除漂流瓶",
         "author": "Todysheep",
         "version": "1.0.0",
     },
 )
```

### Comparing `nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/config.py` & `nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/data_source.py` & `nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py` & `nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.1.2/nonebot_plugin_bottle/model.py` & `nonebot_plugin_bottle-1.0.1.3/nonebot_plugin_bottle/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.1.2/pyproject.toml` & `nonebot_plugin_bottle-1.0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "nonebot_plugin_bottle"
-version = "1.0.1.2"
+version = "1.0.1.3"
 description = "Bottle post plugin in Nonebot"
 authors = ["Todysheep <todysheep@163.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Todysheep/nonebot_plugin_bottle"
 repository = "https://github.com/Todysheep/nonebot_plugin_bottle"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = {extras = ["fastapi"], version = "^2.0.0rc1"}
+nonebot2 = {extras = ["fastapi"], version = "^2.0.0"}
 nonebot-adapter-onebot = ">=2.2.0"
 aiofiles = ">=0.8.0"
 nonebot-plugin-datastore = ">=0.6.0"
 httpx = ">=0.23.0"
 
 [tool.black]
 line-length = 88
```

### Comparing `nonebot_plugin_bottle-1.0.1.2/PKG-INFO` & `nonebot_plugin_bottle-1.0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 1.0.1.2
+Version: 1.0.1.3
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 License: GNU GPLv3
 Author: Todysheep
 Author-email: todysheep@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.8.0)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.0)
 Requires-Dist: nonebot-plugin-datastore (>=0.6.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0rc1,<3.0.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/Todysheep/nonebot_plugin_bottle
 Description-Content-Type: text/markdown
 
 # Nonebot 漂流瓶插件
 * 安装
     -
     - 使用 `pip install nonebot_plugin_bottle`
```

