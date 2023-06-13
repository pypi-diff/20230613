# Comparing `tmp/mvtech-plugin-1.0.7.tar.gz` & `tmp/mvtech-plugin-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mvtech-plugin-1.0.7.tar", last modified: Fri Jun  9 01:03:56 2023, max compression
+gzip compressed data, was "dist\mvtech-plugin-1.0.8.tar", last modified: Tue Jun 13 07:14:40 2023, max compression
```

## Comparing `mvtech-plugin-1.0.7.tar` & `mvtech-plugin-1.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.604062 mvtech-plugin-1.0.7/
--rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2680 2023-06-09 01:03:56.604062 mvtech-plugin-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2403 2023-06-09 01:03:19.000000 mvtech-plugin-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.588102 mvtech-plugin-1.0.7/core/
--rw-rw-rw-   0        0        0       21 2023-06-09 01:03:32.000000 mvtech-plugin-1.0.7/core/__init__.py
--rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.7/core/cli_methods.py
--rw-rw-rw-   0        0        0    14629 2023-06-07 07:38:51.000000 mvtech-plugin-1.0.7/core/config.py
--rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.7/core/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.589104 mvtech-plugin-1.0.7/core/res/
-drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.598084 mvtech-plugin-1.0.7/core/res/SDK/
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.7/core/res/SDK/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.7/core/res/SDK/base.py
--rw-rw-rw-   0        0        0     2126 2023-06-07 03:13:07.000000 mvtech-plugin-1.0.7/core/res/SDK/cli.py
--rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.7/core/res/SDK/http_run.py
--rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.7/core/res/SDK/models.py
--rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.7/core/res/SDK/plugin.py
--rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.7/core/res/SDK/run_define.py
--rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.7/core/res/SDK/service_stop.py
--rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.7/core/res/SDK/web.py
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.7/core/res/__init__.py
--rw-rw-rw-   0        0        0    38085 2023-06-09 00:58:19.000000 mvtech-plugin-1.0.7/core/res/project.tar.gz
--rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.7/core/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.604062 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/
--rw-rw-rw-   0        0        0     2680 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 01:03:56.605214 mvtech-plugin-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:14:40.388223 mvtech-plugin-1.0.8/
+-rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2920 2023-06-13 07:14:40.388223 mvtech-plugin-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-06-13 06:53:26.000000 mvtech-plugin-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 07:14:40.370272 mvtech-plugin-1.0.8/core/
+-rw-rw-rw-   0        0        0       21 2023-06-13 07:13:46.000000 mvtech-plugin-1.0.8/core/__init__.py
+-rw-rw-rw-   0        0        0     9223 2023-06-13 07:09:10.000000 mvtech-plugin-1.0.8/core/cli_methods.py
+-rw-rw-rw-   0        0        0     9664 2023-06-13 06:46:46.000000 mvtech-plugin-1.0.8/core/demo_constants.py
+-rw-rw-rw-   0        0        0      991 2023-06-13 01:11:24.000000 mvtech-plugin-1.0.8/core/main.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:14:40.371269 mvtech-plugin-1.0.8/core/res/
+drwxrwxrwx   0        0        0        0 2023-06-13 07:14:40.381241 mvtech-plugin-1.0.8/core/res/SDK/
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.8/core/res/SDK/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.8/core/res/SDK/base.py
+-rw-rw-rw-   0        0        0     2126 2023-06-07 03:13:07.000000 mvtech-plugin-1.0.8/core/res/SDK/cli.py
+-rw-rw-rw-   0        0        0     4528 2023-06-13 01:05:14.000000 mvtech-plugin-1.0.8/core/res/SDK/http_run.py
+-rw-rw-rw-   0        0        0      159 2023-06-13 06:51:49.000000 mvtech-plugin-1.0.8/core/res/SDK/models.py
+-rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.8/core/res/SDK/plugin.py
+-rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.8/core/res/SDK/run_define.py
+-rw-rw-rw-   0        0        0     1681 2023-06-13 06:34:12.000000 mvtech-plugin-1.0.8/core/res/SDK/service_stop.py
+-rw-rw-rw-   0        0        0     5345 2023-06-13 06:46:11.000000 mvtech-plugin-1.0.8/core/res/SDK/web.py
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.8/core/res/__init__.py
+-rw-rw-rw-   0        0        0    38001 2023-06-13 06:48:59.000000 mvtech-plugin-1.0.8/core/res/project.tar.gz
+-rw-rw-rw-   0        0        0     3539 2023-06-13 07:09:10.000000 mvtech-plugin-1.0.8/core/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:14:40.387227 mvtech-plugin-1.0.8/mvtech_plugin.egg-info/
+-rw-rw-rw-   0        0        0     2920 2023-06-13 07:14:40.000000 mvtech-plugin-1.0.8/mvtech_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-06-13 07:14:40.000000 mvtech-plugin-1.0.8/mvtech_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:14:40.000000 mvtech-plugin-1.0.8/mvtech_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-13 07:14:40.000000 mvtech-plugin-1.0.8/mvtech_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2023-06-13 07:14:40.000000 mvtech-plugin-1.0.8/mvtech_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 07:14:40.000000 mvtech-plugin-1.0.8/mvtech_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:14:40.389220 mvtech-plugin-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.8/setup.py
```

### Comparing `mvtech-plugin-1.0.7/PKG-INFO` & `mvtech-plugin-1.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: mvtech-plugin
-Version: 1.0.7
-Summary: 插件生成等功能...
-Home-page: https://www.mvtech.cn/market/introduction
-Author: sandy
-Author-email: tong@mvtech.com.cn
-License: MIT
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 ### mvtech_plugin
 
 ---
 
 #### 简介
 
 **mvtech_plugin**是MVTech插件脚手架
@@ -26,21 +15,22 @@
 │   ├── ???.py     
 │   ├── models.py
 ├── Dockerfile
 ├── help.md
 ├── icon.png
 ├── main.py
 ├── Makefile
-├── ?_plugin.yaml
+├── plugin.yaml
 ├── requirements.txt
 ├── make_image.sh
 ├── SDK
+│   ├── __init__.py
 │   ├── base.py
 │   ├── cli.py
-│   ├── __init__.py
+│   ├── http_run.py
 │   ├── models.py
 │   ├── plugin.py
 │   ├── run_define.py
 │   └── web.py
 ├── testAPI.py
 │   ├── ???.json
 └── triggers
@@ -112,7 +102,18 @@
 make tarball
 
 #### 离线打Docker包
 
 - docker save <myimage>:<tag> | gzip > <myimage>_<tag>.tar.gz
 
 - docker save mvtech/rest:1.0.0 | gzip > mvtech_rest_1.0.0.tar.gz
+
+#### 属性类型定义
+* "string": "str",
+* "bytes": "str",
+*  "boolean": "bool",
+*  "float": "float",
+* "date": "str",
+* "object": "dict",
+* "password": "str",
+* "integer": "int",
+* "file": "dict"
```

### Comparing `mvtech-plugin-1.0.7/core/cli_methods.py` & `mvtech-plugin-1.0.8/core/cli_methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from core.config import *
+from core.demo_constants import *
 from core.tools import Tools
 import logging
 
 tools = Tools()
 
 
 def generate(path: str, yml: str):
@@ -16,21 +16,19 @@
     yml_path = os.path.join(path, yml)
     if not any([yml.endswith(y)
                 for y in ["yml", "yaml"]]) or not os.path.exists(yml_path):
         logging.error(f"yaml路径错误 - {yml_path}")
         return
     else:
         yaml_data = tools.readYaml(yml_path)
-        logging.info(f"readed {yml}")
+        logging.info(f"look {yml}")
 
-    plugin_name = yaml_data.get("name", "hah")
+    plugin_name = yaml_data.get("name", "mvtechname")
     actions_class_list = []
     triggers_class_list = []
-    indicator_receivers_class_list = []
-    alarm_receivers_class_list = []
 
     # 当前文件路劲下生成sdk
     tar_path = os.path.join(BASE_DIR, os.path.join("res", "project.tar.gz"))
     target_path = path
     tools.tarExtract(tar_path, target_path)
 
     # 读取types
@@ -38,23 +36,23 @@
     typesTemp = ""
     if types:
         for types_name, types_data in types.items():
             typesData = {
                 "className": tools.getModelName(types_name),
                 "args": tools.ymlTransPy(types_data)
             }
-            typesTemp += tools.renderStrTemplate(typesData, MODELTEMPLATE)
+            typesTemp += tools.renderStrTemplate(typesData, MODEL_INFO)
 
     # 读取adapter
     adapter = yaml_data.get("adapter")
     adapter = {
         "className": tools.getModelName("adapter"),
         "args": tools.ymlTransPy(adapter)
     }
-    connTemp = tools.renderStrTemplate(adapter, MODELTEMPLATE)
+    connTemp = tools.renderStrTemplate(adapter, MODEL_INFO)
 
     # 创建tests
     tests_path = os.path.join(path, "tests")
     if not os.path.exists(tests_path):
         os.mkdir(tests_path)
 
     # 生成actions
@@ -90,16 +88,16 @@
                 "args": tools.ymlTransPy(inp)
             }
             outp_data = {
                 "className": outpClassName,
                 "args": tools.ymlTransPy(outp)
             }
 
-            inpTemp = tools.renderStrTemplate(inp_data, MODELTEMPLATE)
-            outpTemp = tools.renderStrTemplate(outp_data, MODELTEMPLATE)
+            inpTemp = tools.renderStrTemplate(inp_data, MODEL_INFO)
+            outpTemp = tools.renderStrTemplate(outp_data, MODEL_INFO)
 
             # model主要内容
             actionsModelTemp += inpTemp
             actionsModelTemp += outpTemp
             actionsModelTemp += BASERUNPARAM
 
             # action
@@ -107,44 +105,44 @@
                 "actionsName": actionsName,
                 "name": title,
                 "inputModel": inpClassName,
                 "outputModel": outpClassName,
                 "baseRunModel": "BASE_RUN_PARAM",
                 "adapMdl": tools.getModelName("adapter"),
             }
-            actionsTemp = tools.renderStrTemplate(actionData, ACTIONTEMPLATE)
+            actionsTemp = tools.renderStrTemplate(actionData, ACTION_INFO)
 
             file_path = os.path.join(actions_path, f"{title}.py")
             if not os.path.exists(file_path):
                 tools.writeFile(actionsTemp, file_path)
-                logging.info(f"gnerated actions/{title}.py ok")
+                logging.info(f"mkdir actions/{title}.py ok")
 
             # 生成测试文件
             file_path = os.path.join(tests_path, f"{title}.json")
             testData = tools.renderStrTemplate({"title": title},
-                                               ACTIONSTESTTEMPLATE)
+                                               ACTION_FAST_API_INFO)
             tools.writeFile(testData, file_path)
-            logging.info(f"generated tests/{title}.json ok")
+            logging.info(f"mkdir tests/{title}.json ok")
 
         # 生成__init__.py
         file_path = os.path.join(actions_path, "__init__.py")
         initData = tools.renderStrTemplate({"init_list": init_list},
-                                           INITTEMPLATE)
+                                           INIT_INFO)
         tools.writeFile(initData, file_path)
-        logging.info(f"generated actions/__init__.py ok")
+        logging.info(f"mkdir actions/__init__.py ok")
 
         file_path = os.path.join(actions_path, "models.py")
         tools.writeFile(actionsModelTemp, file_path)
-        logging.info(f"gnerated actions/models.py ok")
+        logging.info(f"mkdir actions/models.py ok")
         # 生成actions的REST 测试接口
         file_path = os.path.join(path, "testAPI.py")
         testAPIData = tools.renderStrTemplate({"init_list": init_list},
-                                              TESTAPITEMPLATE)
+                                              FAST_API_INFO)
         tools.writeFile(testAPIData, file_path)
-        logging.info(f"generated testAPI.py ok")
+        logging.info(f"mkdir testAPI.py ok")
 
         #===
     #===
 
     # 生成triggers
     triggers = yaml_data.get("triggers")
     if triggers:
@@ -178,81 +176,81 @@
                 "args": tools.ymlTransPy(inp)
             }
             outp_data = {
                 "className": outpClassName,
                 "args": tools.ymlTransPy(outp)
             }
 
-            inpTemp = tools.renderStrTemplate(inp_data, MODELTEMPLATE)
-            outpTemp = tools.renderStrTemplate(outp_data, MODELTEMPLATE)
+            inpTemp = tools.renderStrTemplate(inp_data, MODEL_INFO)
+            outpTemp = tools.renderStrTemplate(outp_data, MODEL_INFO)
 
             # model主要内容
             triggersModelTemp += inpTemp
             triggersModelTemp += outpTemp
 
             # trigger
             triggerData = {
                 "triggersName": triggersName,
                 "name": title,
                 "inputModel": inpClassName,
                 "outputModel": outpClassName,
                 "adapMdl": tools.getModelName("adapter"),
             }
             triggersTemp = tools.renderStrTemplate(triggerData,
-                                                   TRIGGERSTEMPLATE)
+                                                   TRIGGER_INFO)
 
             file_path = os.path.join(triggers_path, f"{title}.py")
             if not os.path.exists(file_path):
                 tools.writeFile(triggersTemp, file_path)
-                logging.info(f"gnerated triggers/{title}.py ok")
+                logging.info(f"mkdir triggers/{title}.py ok")
 
             # 生成测试文件
             file_path = os.path.join(tests_path, f"{title}.json")
             testData = tools.renderStrTemplate({"title": title},
-                                               TRIGGERSTESTTEMPLATE)
+                                               TRIGGER_FAST_API_INFO)
             tools.writeFile(testData, file_path)
-            logging.info(f"generated tests/{title}.json ok")
+            logging.info(f"mkdir tests/{title}.json ok")
 
         # 生成__init__.py
         file_path = os.path.join(triggers_path, "__init__.py")
         initData = tools.renderStrTemplate({"init_list": init_list},
-                                           INITTEMPLATE)
+                                           INIT_INFO)
         tools.writeFile(initData, file_path)
-        logging.info(f"generated triggers/__init__.py ok")
+        logging.info(f"mkdir triggers/__init__.py ok")
 
         file_path = os.path.join(triggers_path, "models.py")
         tools.writeFile(triggersModelTemp, file_path)
-        logging.info(f"gnerated triggers/models.py ok")
+        logging.info(f"mkdir triggers/models.py ok")
 
     #===
 
     # 创建入口文件　main.py
     mainData = {
         "pluginName": tools.getModelName(plugin_name,
                                          "Plugin").replace(" ", "_"),
         "actionClassees": actions_class_list,
         "triggerClassees": triggers_class_list
     }
     file_path = os.path.join(path, "main.py")
-    mainTemp = tools.renderStrTemplate(mainData, MAINTEMPLATE)
+    mainTemp = tools.renderStrTemplate(mainData, MAIN_INFO)
     tools.writeFile(mainTemp, file_path)
-    logging.info(f"generated main.py ok")
+    logging.info(f"mkdir main.py ok")
 
     # 创建help.md
     helpData = yaml_data
     file_path = os.path.join(path, "help.md")
-    mainTemp = tools.renderStrTemplate(helpData, HELPTEMPLATE)
+    mainTemp = tools.renderStrTemplate(helpData, HELP_INFO)
     tools.writeFile(mainTemp, file_path)
-    logging.info("generated help.md ok")
+    logging.info("mkdir help.md ok")
 
     # 生成util
     util_path = os.path.join(path, "util")
     if not os.path.exists(util_path):
         os.mkdir(util_path)
-        logging.info("generated util ok")
+        logging.info("mkdir util ok")
 
     logging.info("^_^!! TemplateSourceCode done ")
 
 
 def run(path: str, tests: str):
 
     main_path = os.path.join(path, "main.py")
@@ -268,31 +266,7 @@
 def http(path: str):
     main_path = os.path.join(path, "main.py")
 
     cmd = f"python {main_path} http"
     os.system(cmd)
 
 
-def test(path: str, tests: str):
-    main_path = os.path.join(path, "main.py")
-    tests_path = os.path.join(path, tests)
-
-    if not os.path.exists(tests_path):
-        logging.error(f"请正确输入路径{tests_path}")
-
-    cmd = f"python {main_path} test < {tests_path}"
-    os.system(cmd)
-
-
-def tarball(path: str):
-
-    Makefile_path = os.path.join(path, "Makefile")
-    if os.path.exists(Makefile_path):
-        cmd = "make tarball"
-        os.system(cmd)
-
-
-def mkimg(path: str):
-    Makefile_path = os.path.join(path, "Makefile")
-    if os.path.exists(Makefile_path):
-        cmd = "make image"
-        os.system(cmd)
```

### Comparing `mvtech-plugin-1.0.7/core/res/SDK/base.py` & `mvtech-plugin-1.0.8/core/res/SDK/base.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.7/core/res/SDK/cli.py` & `mvtech-plugin-1.0.8/core/res/SDK/cli.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.7/core/res/SDK/http_run.py` & `mvtech-plugin-1.0.8/core/res/SDK/http_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,15 @@
     log("info", "检测需要运行的组件")
     #   检查json数据是使用在哪个组件上的
     if data_body.get("action"):
         runAction(data_body["action"], data_body, plugin_object)
 
     elif data_body.get("trigger"):
         runTrigger(data_body["trigger"], data_body, plugin_object)
-
-    elif data_body.get("receiver"):
-        runIndicatorReceiver(data_body["receiver"], data_body, plugin_object)
+ 
 
     else:
         log("info", "未检测到需要运行的组件")
 
 
 def runAction(action_name: str, data: dict, plugin_object):
     """
```

### Comparing `mvtech-plugin-1.0.7/core/res/SDK/run_define.py` & `mvtech-plugin-1.0.8/core/res/SDK/run_define.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.7/core/res/SDK/service_stop.py` & `mvtech-plugin-1.0.8/core/res/SDK/service_stop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 from threading import Timer
 # import asyncio
-# from uvicorn import Config, Server
 import uvicorn
 try:
     from .base import log
 except Exception: 
     from base import log
 import sys, os
 # 服务是否有未运行完的action
```

### Comparing `mvtech-plugin-1.0.7/core/res/SDK/web.py` & `mvtech-plugin-1.0.8/core/res/SDK/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi import FastAPI
 import typing
 import uvicorn
 import asyncio
 import threading
-# from uvicorn import Config, Server
+# from uvicorn import demo_constants, Server
 try:
     from . import models
     from .base import clearLog, checkModel, log, getLog, checkTriggerModel
     from .service_stop import start_live, live_add, live_sub
 except Exception:
     import models
     from base import clearLog, checkModel, log, getLog, checkTriggerModel
@@ -149,17 +149,17 @@
 
         output = trigger._test(adapter_data)
 
         return output
 
     def runserver(self):
         portV = 8888
-        log("info", f"mvtech web start  http://0.0.0.0:{portV}/docs#")
-        # config = uvicorn.Config(app, host="0.0.0.0", port=portV, log_level="info", loop="asyncio")
-        config = uvicorn.Config(app, host="0.0.0.0", port=portV, log_level="info")
+        log("info", f"mvtech web start  http://127.0.0.1:{portV}/docs#")
+        # config = uvicorn.Config(app, host="127.0.0.1", port=portV, log_level="info", loop="asyncio")
+        ser_config = uvicorn.Config(app, host="127.0.0.1", port=portV, log_level="info")
         global userver
-        userver = uvicorn.Server(config=config) 
+        userver = uvicorn.Server(config=ser_config) 
         # start_live(userver)
         userver.run()
```

### Comparing `mvtech-plugin-1.0.7/core/res/project.tar.gz` & `mvtech-plugin-1.0.8/core/res/project.tar.gz`

 * *Files 23% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Jun  9 00:58:14 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, last modified: Tue Jun 13 06:48:55 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

#### project.tar

##### file list

```diff
@@ -2,15 +2,15 @@
 -rw-r--r--   0 andy      (1000) andy      (1000)    29297 2021-07-26 09:20:11.000000 ./icon.png
 -rwxrwxrwx   0        0        0      897 2023-06-06 01:53:59.000000 ./Makefile
 -rwxrwxrwx   0        0        0      825 2023-06-07 09:25:12.000000 ./make_image.sh
 -rwxr-xr-x   0 andy      (1000) andy      (1000)       66 2021-07-27 01:47:24.000000 ./requirements.txt
 drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2021-11-18 04:18:06.000000 ./SDK/
 -rwxrwxrwx   0        0        0     7829 2023-02-15 05:39:36.000000 ./SDK/base.py
 -rwxrwxrwx   0        0        0     2132 2023-06-05 07:27:02.000000 ./SDK/cli.py
--rwxrwxrwx   0        0        0     5874 2023-02-20 06:58:57.000000 ./SDK/http_run.py
+-rwxrwxrwx   0        0        0     4528 2023-06-13 01:05:14.000000 ./SDK/http_run.py
 -rwxrwxrwx   0        0        0      162 2023-03-27 00:44:29.000000 ./SDK/models.py
 -rwxrwxrwx   0        0        0      462 2023-03-27 00:41:14.000000 ./SDK/plugin.py
 -rwxrwxrwx   0        0        0    12776 2023-06-05 09:23:34.000000 ./SDK/run_define.py
--rwxrwxrwx   0        0        0     1719 2023-02-20 08:33:11.000000 ./SDK/service_stop.py
--rwxrwxrwx   0        0        0     5323 2023-06-05 09:24:15.000000 ./SDK/web.py
+-rwxrwxrwx   0        0        0     1681 2023-06-13 06:34:12.000000 ./SDK/service_stop.py
+-rwxrwxrwx   0        0        0     5345 2023-06-13 06:46:11.000000 ./SDK/web.py
 -rwxrwxrwx   0        0        0        0 2023-01-29 09:23:09.000000 ./SDK/__init__.py
 -rw-r--r--   0 andy      (1000) andy      (1000)        0 2021-07-26 10:10:45.000000 ./__init__.py
```

##### ./SDK/http_run.py

```diff
@@ -26,17 +26,15 @@
     log("info", "检测需要运行的组件")
     #   检查json数据是使用在哪个组件上的
     if data_body.get("action"):
         runAction(data_body["action"], data_body, plugin_object)
 
     elif data_body.get("trigger"):
         runTrigger(data_body["trigger"], data_body, plugin_object)
-
-    elif data_body.get("receiver"):
-        runIndicatorReceiver(data_body["receiver"], data_body, plugin_object)
+ 
 
     else:
         log("info", "未检测到需要运行的组件")
 
 
 def runAction(action_name: str, data: dict, plugin_object):
     """
@@ -94,51 +92,14 @@
         next_step = data.get("nextStep")
 
         trigger._run(input_data, adapter_data, next_step)
 
     log("info", "触发器(Trigger) 运行结束")
 
 
-
-def runIndicatorReceiver(indicator_receiver_name: str, data: dict,
-                         plugin_object):
-    """
-    #   运行情报接收器
-    参数说明：
-    action_name:str,    #动作名
-    data:dict,      #   运行功能时的必要的数据
-    plugin_object:PLUGIN,      #   插件集合对象（类位于生成的插件后的根目录下main.py文件内）
-
-    出现异常时，会将异常信息放入log，但不会抛出异常
-    """
-    log("info", "运行 情报接收器(IndicatorReceiver) 中")
-
-    enable_web = data.get("enable_web")
-
-    #   使用web服务
-    if enable_web:
-
-        server = Server(plugin_object)
-        server.runserver()
-
-    else:
-        #   根据动作名在插件根目录下的 main.py 文件内的动作列表内选取对应的动作类，并初始化一个对象
-        indicator_receiver = plugin_object.indicator_receivers[
-            indicator_receiver_name]
-
-        adapter_data = data.get("adapter")
-
-        input_data = data.get("input")
-        next_step = data.get("nextStep")
-
-        indicator_receiver._run(input_data, adapter_data, next_step)
-
-    log("info", "情报接收器(IndicatorReceiver) 运行结束")
-
-
 def test(data: dict, plugin_object):
     """
     #   只运行连接器部分
     参数说明：
     data:dict,      #   运行功能时的必要的json数据
     plugin_object:PLUGIN,      #   插件集合对象（类位于生成的插件后的根目录下main.py文件内）
     """
```

##### ./SDK/service_stop.py

```diff
@@ -1,11 +1,10 @@
 
 from threading import Timer
 # import asyncio
-# from uvicorn import Config, Server
 import uvicorn
 try:
     from .base import log
 except Exception: 
     from base import log
 import sys, os
 # 服务是否有未运行完的action
```

##### ./SDK/web.py

```diff
@@ -1,13 +1,13 @@
 from fastapi import FastAPI
 import typing
 import uvicorn
 import asyncio
 import threading
-# from uvicorn import Config, Server
+# from uvicorn import demo_constants, Server
 try:
     from . import models
     from .base import clearLog, checkModel, log, getLog, checkTriggerModel
     from .service_stop import start_live, live_add, live_sub
 except Exception:
     import models
     from base import clearLog, checkModel, log, getLog, checkTriggerModel
@@ -149,17 +149,17 @@
 
         output = trigger._test(adapter_data)
 
         return output
 
     def runserver(self):
         portV = 8888
-        log("info", f"mvtech web start  http://0.0.0.0:{portV}/docs#")
-        # config = uvicorn.Config(app, host="0.0.0.0", port=portV, log_level="info", loop="asyncio")
-        config = uvicorn.Config(app, host="0.0.0.0", port=portV, log_level="info")
+        log("info", f"mvtech web start  http://127.0.0.1:{portV}/docs#")
+        # config = uvicorn.Config(app, host="127.0.0.1", port=portV, log_level="info", loop="asyncio")
+        ser_config = uvicorn.Config(app, host="127.0.0.1", port=portV, log_level="info")
         global userver
-        userver = uvicorn.Server(config=config) 
+        userver = uvicorn.Server(config=ser_config) 
         # start_live(userver)
         userver.run()
```

### Comparing `mvtech-plugin-1.0.7/core/tools.py` & `mvtech-plugin-1.0.8/core/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import tarfile
 import yaml
 import jinja2
 from typing import List, Optional, Any
 import os
-
-
-from core.config import *
+import logging
+logging.basicConfig(level=logging.DEBUG, format="%(levelname)s | %(message)s")
 
 
 class Tools(object):
 
     def tarExtract(self, tar_path, target_path):
         """
-        .tar.gz　提取
+        获取 包内容
         """
 
         try:
             tar = tarfile.open(tar_path, "r:gz")
             file_names = tar.getnames()
             for file_name in file_names:
                 if not os.path.exists(os.path.join(target_path, file_name)):
@@ -87,15 +86,15 @@
         py_list = []
 
         if data:
             for name,v in data.items():
                 # 默认　type: string, required: false
                 tp = v.get("type", "string")
                 rq = v.get("required", False)
-                dft = v.get("default", None)
+                dft = v.get("defaultv", None)
                 enm = v.get("enum", None)
 
                 assert not (isinstance(enm, list) and dft and dft not in enm), "valid fail, default value not in enum value."
 
                 tp = self.typeTrans(tp, rq, dft, enm)
 
                 py_list.append([name, tp])
```

### Comparing `mvtech-plugin-1.0.7/mvtech_plugin.egg-info/PKG-INFO` & `mvtech-plugin-1.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.7
+Version: 1.0.8
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -26,21 +26,22 @@
 │   ├── ???.py     
 │   ├── models.py
 ├── Dockerfile
 ├── help.md
 ├── icon.png
 ├── main.py
 ├── Makefile
-├── ?_plugin.yaml
+├── plugin.yaml
 ├── requirements.txt
 ├── make_image.sh
 ├── SDK
+│   ├── __init__.py
 │   ├── base.py
 │   ├── cli.py
-│   ├── __init__.py
+│   ├── http_run.py
 │   ├── models.py
 │   ├── plugin.py
 │   ├── run_define.py
 │   └── web.py
 ├── testAPI.py
 │   ├── ???.json
 └── triggers
@@ -112,7 +113,18 @@
 make tarball
 
 #### 离线打Docker包
 
 - docker save <myimage>:<tag> | gzip > <myimage>_<tag>.tar.gz
 
 - docker save mvtech/rest:1.0.0 | gzip > mvtech_rest_1.0.0.tar.gz
+
+#### 属性类型定义
+* "string": "str",
+* "bytes": "str",
+*  "boolean": "bool",
+*  "float": "float",
+* "date": "str",
+* "object": "dict",
+* "password": "str",
+* "integer": "int",
+* "file": "dict"
```

### Comparing `mvtech-plugin-1.0.7/mvtech_plugin.egg-info/SOURCES.txt` & `mvtech-plugin-1.0.8/mvtech_plugin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 core/__init__.py
 core/cli_methods.py
-core/config.py
+core/demo_constants.py
 core/main.py
 core/tools.py
 core/res/__init__.py
 core/res/project.tar.gz
 core/res/SDK/__init__.py
 core/res/SDK/base.py
 core/res/SDK/cli.py
```

### Comparing `mvtech-plugin-1.0.7/setup.py` & `mvtech-plugin-1.0.8/setup.py`

 * *Files identical despite different names*

