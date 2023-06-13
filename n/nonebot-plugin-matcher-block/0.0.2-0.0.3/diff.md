# Comparing `tmp/nonebot_plugin_matcher_block-0.0.2.tar.gz` & `tmp/nonebot_plugin_matcher_block-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_matcher_block-0.0.2.tar", last modified: Tue Feb  7 18:09:46 2023, max compression
+gzip compressed data, was "nonebot_plugin_matcher_block-0.0.3.tar", last modified: Tue Jun 13 13:40:43 2023, max compression
```

## Comparing `nonebot_plugin_matcher_block-0.0.2.tar` & `nonebot_plugin_matcher_block-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 18:09:46.556656 nonebot_plugin_matcher_block-0.0.2/
--rw-rw-rw-   0        0        0     1086 2022-12-05 12:34:39.000000 nonebot_plugin_matcher_block-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      284 2023-02-07 18:09:46.556156 nonebot_plugin_matcher_block-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-07 18:09:46.547148 nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block/
--rw-rw-rw-   0        0        0     6740 2023-02-07 18:07:11.000000 nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-07 18:09:46.555154 nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block.egg-info/
--rw-rw-rw-   0        0        0      284 2023-02-07 18:09:46.000000 nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-02-07 18:09:46.000000 nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 18:09:46.000000 nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-02-07 18:09:46.000000 nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-02-07 18:09:46.000000 nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-07 18:09:46.557156 nonebot_plugin_matcher_block-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      530 2023-02-07 18:09:43.000000 nonebot_plugin_matcher_block-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:40:43.460952 nonebot_plugin_matcher_block-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2022-12-05 12:34:39.000000 nonebot_plugin_matcher_block-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      284 2023-06-13 13:40:43.460452 nonebot_plugin_matcher_block-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 13:40:43.451944 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block/
+-rw-rw-rw-   0        0        0     7160 2023-06-13 13:35:48.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:40:43.458950 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 13:40:43.460952 nonebot_plugin_matcher_block-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      530 2023-06-13 13:40:39.000000 nonebot_plugin_matcher_block-0.0.3/setup.py
```

### Comparing `nonebot_plugin_matcher_block-0.0.2/LICENSE` & `nonebot_plugin_matcher_block-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_matcher_block-0.0.2/nonebot_plugin_matcher_block/__init__.py` & `nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from nonebot.plugin.on import on_message, on_command
+from nonebot.plugin.on import on_command
 from nonebot.matcher import Matcher
 from nonebot.adapters.onebot.v11 import (
     GROUP_ADMIN,
     GROUP_OWNER,
+    Bot,
     GroupMessageEvent,
     Message,
-    MessageSegment
     )
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
 from pathlib import Path
 
 import time
@@ -29,56 +29,50 @@
 time_config_file = path / "time_config.json"
 
 if time_config_file.exists():
     with open(time_config_file, "r", encoding="utf8") as f:
         time_config = json.load(f)
 else:
     time_config = {}
-    with open(time_config_file, "w", encoding="utf8") as f:
-        json.dump({}, f, ensure_ascii=False, indent=4)
-
 
 group_config_file = path / "group_config.json"
 
 if group_config_file.exists():
     with open(group_config_file, "r", encoding="utf8") as f:
         group_config = json.load(f)
 else:
     group_config = {}
-    with open(group_config_file, "w", encoding="utf8") as f:
-        json.dump({}, f, ensure_ascii=False, indent=4)
-
-cache = {}
 
-def is_block_group(event: GroupMessageEvent) -> bool:
+def is_block_group(event:GroupMessageEvent) -> bool:
     msg = str(event.message)
     for command in set(group_config.keys()):
-        if command.startswith("^") and command.endswith("$"):
+        if command.startswith("^"):
             if re.match(re.compile(command),msg):
                 break
             else:
                 continue
         else:
             if msg.startswith(command):
                 break
             else:
                 continue
     else:
         return False
     group_id = event.group_id
     if group_id in group_config[command]:
-        event.raw_message = ""
         return True
     else:
         return False
 
-def is_block_time(event: GroupMessageEvent) -> bool:
+cache = {}
+
+def is_block_time(event:GroupMessageEvent) -> bool:
     msg = str(event.message)
     for command in set(time_config.keys()):
-        if command.startswith("^") and command.endswith("$"):
+        if command.startswith("^"):
             if re.match(re.compile(command),msg):
                 break
             else:
                 continue
         else:
             if msg.startswith(command):
                 break
@@ -91,31 +85,27 @@
     user_id = event.user_id
     cache.setdefault(group_id,{})
     cd = time.time() - cache[group_id].get(user_id,0)
     if cd > time_config[command]:
         cache[group_id][user_id] = time.time()
         return False
     else:
-        event.raw_message = f"你的【{command}】冷却还有{int(time_config[command] - cd) + 1}秒"
-        return True
+        return f"你的【{command}】冷却还有{int(time_config[command] - cd) + 1}秒"
 
-async def is_block(event: GroupMessageEvent) -> bool:
-    return is_block_group(event) or is_block_time(event)
-
-block = on_message(rule = is_block, priority = 0, block = False)
-
-@block.handle()
-async def _(matcher: Matcher,event:GroupMessageEvent):
-    matcher.stop_propagation()
-    msg = event.raw_message
-    if msg:
-        await block.finish(msg,at_sender = True)
-    else:
-        await block.finish()
+from nonebot.message import event_preprocessor
+from nonebot.exception import IgnoredException
 
+@event_preprocessor
+async def do_something(bot:Bot, event:GroupMessageEvent , permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER):
+    if not await permission(bot,event):
+        if is_block_group(event):
+            raise IgnoredException("本群已屏蔽此指令")
+        if echo := is_block_time(event):
+            await bot.send(event = event, message = echo)
+            raise IgnoredException("用户指令正在冷却")
 
 add_block = on_command("添加阻断", permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER, priority = 5, block = True)
 
 @add_block.handle()
 async def _(matcher: Matcher, event:GroupMessageEvent, arg: Message = CommandArg()):
     msg = arg.extract_plain_text().strip().split()
     if msg and len(msg) >= 2:
@@ -180,8 +170,30 @@
     msg = ""
     for command in set(group_config.keys()):
         if group_id in group_config[command]:
             msg += f"【{command}】：屏蔽\n"
     for command in set(time_config.keys()):
         msg += f"【{command}】：{time_config[command]}s\n"
 
-    await show_block.finish(msg[:-1])
+    await show_block.finish(msg[:-1])
+
+from nonebot import get_driver
+
+driver = get_driver()
+bot_list = set()
+driver.on_bot_connect(lambda bot:bot_list.add(int(bot.self_id)))
+driver.on_bot_disconnect(lambda bot:bot_list.discard(int(bot.self_id)))
+
+history = []
+
+@event_preprocessor
+async def do_something(event: GroupMessageEvent):
+    if len(bot_list) > 1:
+        if event.user_id in bot_list:
+            raise IgnoredException("event来自其他bot")
+        global history
+        history = history[:20]
+        message_id = event.message_id
+        if message_id in history:
+            raise IgnoredException("event已被其他bot处理")
+        else:
+            history.insert(0, message_id)
```

### Comparing `nonebot_plugin_matcher_block-0.0.2/setup.py` & `nonebot_plugin_matcher_block-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_matcher_block',
-version='0.0.2',
+version='0.0.3',
 description='通用指令阻断',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_matcher_block"]),
```

