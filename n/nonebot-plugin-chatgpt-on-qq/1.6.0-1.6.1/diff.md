# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.6.0.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.6.0.tar", last modified: Sun May 14 08:13:21 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.6.1.tar", last modified: Tue Jun 13 04:36:04 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0.tar` & `nonebot-plugin-chatgpt-on-qq-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:13:21.635310 nonebot-plugin-chatgpt-on-qq-1.6.0/
--rw-rw-rw-   0        0        0      770 2023-05-14 08:13:21.632310 nonebot-plugin-chatgpt-on-qq-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 08:13:21.589033 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    21829 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     1293 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
--rw-rw-rw-   0        0        0    12934 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/sessions.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:13:21.626311 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      770 2023-05-14 08:13:19.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-05-14 08:13:20.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:13:19.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-05-14 08:13:19.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-14 08:13:19.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 08:13:21.635310 nonebot-plugin-chatgpt-on-qq-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-05-14 08:11:32.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:36:04.369549 nonebot-plugin-chatgpt-on-qq-1.6.1/
+-rw-rw-rw-   0        0        0      770 2023-06-13 04:36:04.367540 nonebot-plugin-chatgpt-on-qq-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 04:36:04.336542 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    22213 2023-06-13 04:30:27.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     1293 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+-rw-rw-rw-   0        0        0    12934 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/sessions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:36:04.361541 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 04:36:04.369549 nonebot-plugin-chatgpt-on-qq-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-06-13 04:32:16.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.6.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.6.0
+Version: 1.6.1
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,41 +17,51 @@
 from nonebot.plugin import PluginMetadata
 
 from .config import Config, plugin_config
 from .loadpresets import presets_str
 from .custom_errors import NeedCreatSession
 from .sessions import session_container, Session, get_group_id
 
+customize_prefix: str = plugin_config.customize_prefix
+customize_talk_cmd: str = plugin_config.customize_talk_cmd
+# 因为电脑端的qq在输入/chat xxx时候经常被转换成表情，所以支持自定义指令前缀替换"chat"
+change_chat_to: str = plugin_config.change_chat_to
+prefix_str = customize_prefix if customize_prefix is not None else '/'
+chat_str = f'(chat|{change_chat_to})' if change_chat_to else 'chat'
+talk_cmd_str = customize_talk_cmd if customize_talk_cmd else 'talk'
+pattern_str = prefix_str + chat_str
+menu_chat_str=prefix_str+f'{change_chat_to}' if change_chat_to else 'chat'
+
 __usage__: str = (
     "指令表：\n"
-    "    /chat help 获取指令帮助菜单\n"
-    "    /chat auth 获取当前群会话管理权限状态\n"
-    "    /chat auth on 设置当前群仅管理员可以管理会话\n"
-    "    /chat auth off 设置当前群所有人均可管理会话\n"
-    "    /talk <会话内容> 在当前会话中进行会话(同样不需要括号，后面直接接你要说的话就行)\n"
+    f"    {menu_chat_str} help 获取指令帮助菜单\n"
+    f"    {menu_chat_str} auth 获取当前群会话管理权限状态\n"
+    f"    {menu_chat_str} auth on 设置当前群仅管理员可以管理会话\n"
+    f"    {menu_chat_str} auth off 设置当前群所有人均可管理会话\n"
+    f"    /talk <会话内容> 在当前会话中进行会话(同样不需要括号，后面直接接你要说的话就行)\n"
     ">> 增\n"
-    "    /chat new  根据预制模板prompt创建并加入一个新的会话\n"
-    "    /chat new <自定义prompt> 根据自定义prompt创建并加入一个新的会话\n"
-    "    /chat json 根据历史会话json来创建一个会话，输入该命令后会提示你在下一个消息中输入json\n"
-    "    /chat cp 根据当前会话创建并加入一个新的会话\n"
-    "    /chat cp <id> 根据会话<id>为模板进行复制新建加入（id为/chat list中的序号）\n"
+    f"    {menu_chat_str} new  根据预制模板prompt创建并加入一个新的会话\n"
+    f"    {menu_chat_str} new <自定义prompt> 根据自定义prompt创建并加入一个新的会话\n"
+    f"    {menu_chat_str} json 根据历史会话json来创建一个会话，输入该命令后会提示你在下一个消息中输入json\n"
+    f"    {menu_chat_str} cp 根据当前会话创建并加入一个新的会话\n"
+    f"    {menu_chat_str} cp <id> 根据会话<id>为模板进行复制新建加入（id为{menu_chat_str} list中的序号）\n"
     ">> 删\n"
-    "    /chat del 删除当前所在会话\n"
-    "    /chat del <id> 删除序号为<id>的会话（id为/chat list中的序号）\n"
-    "    /chat clear 清空本群全部会话\n"
-    "    /chat clear <@user> 删除@用户创建的会话\n"
+    f"    {menu_chat_str} del 删除当前所在会话\n"
+    f"    {menu_chat_str} del <id> 删除序号为<id>的会话（id为{menu_chat_str} list中的序号）\n"
+    f"    {menu_chat_str} clear 清空本群全部会话\n"
+    f"    {menu_chat_str} clear <@user> 删除@用户创建的会话\n"
     ">> 改\n"
-    "    /chat join <id> 加入会话（id为/chat list中的序号）\n"
-    "    /chat rename <name> 重命名当前会话\n"
+    f"    {menu_chat_str} join <id> 加入会话（id为{menu_chat_str} list中的序号）\n"
+    f"    {menu_chat_str} rename <name> 重命名当前会话\n"
     ">> 查\n"
-    "    /chat who 查看当前会话信息\n"
-    "    /chat list 获取当前群所有存在的会话的序号及创建时间\n"
-    "    /chat list <@user> 获取当前群查看@的用户创建的会话\n"
-    "    /chat prompt 查看当前会话的prompt\n"
-    "    /chat dump 导出当前会话json字符串格式的上下文信息，可以用于/chat json导入\n"
+    f"    {menu_chat_str} who 查看当前会话信息\n"
+    f"    {menu_chat_str} list 获取当前群所有存在的会话的序号及创建时间\n"
+    f"    {menu_chat_str} list <@user> 获取当前群查看@的用户创建的会话\n"
+    f"    {menu_chat_str} prompt 查看当前会话的prompt\n"
+    f"    {menu_chat_str} dump 导出当前会话json字符串格式的上下文信息，可以用于{menu_chat_str} json导入\n"
 
 )
 __plugin_meta__ = PluginMetadata(
     name="多功能ChatGPT插件",
     description="基于chatGPT-3.5-turbo API的nonebot插件",
     usage=__usage__,
     config=Config,
@@ -64,23 +74,16 @@
 
 allow_private: bool = plugin_config.allow_private
 api_keys: List[str] = session_container.api_keys
 temperature: float = plugin_config.temperature
 model: str = plugin_config.model_name
 max_tokens: int = plugin_config.max_tokens
 auto_create_preset_info: bool = plugin_config.auto_create_preset_info
-customize_prefix: str = plugin_config.customize_prefix
-customize_talk_cmd: str = plugin_config.customize_talk_cmd
 
-# 因为电脑端的qq在输入/chat xxx时候经常被转换成表情，所以支持自定义指令前缀替换"chat"
-change_chat_to: str = plugin_config.change_chat_to
-prefix_str = customize_prefix if customize_prefix is not None else '/'
-chat_str = f'(chat|{change_chat_to})' if change_chat_to else 'chat'
-talk_cmd_str = customize_talk_cmd if customize_talk_cmd else 'talk'
-pattern_str = prefix_str + chat_str
+
 
 
 async def _allow_private_checker(event: MessageEvent) -> bool:
     return isinstance(event, GroupMessageEvent) or allow_private
 
 
 ALLOW_PRIVATE = Permission(_allow_private_checker)
@@ -188,15 +191,15 @@
 @ChatCP.handle()
 async def _(bot: Bot, event: MessageEvent):
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     await auth_check(ChatCP, bot, event, group_id)
     group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if user_id not in group_usage:
-        await ChatCP.finish('请先加入一个会话，再进行复制当前会话 或者使用 /chat cp <id> 进行复制')
+        await ChatCP.finish(f'请先加入一个会话，再进行复制当前会话 或者使用 {menu_chat_str} cp <id> 进行复制')
     session: Session = group_usage[user_id]
     group_usage[user_id].del_user(user_id)
     new_session: Session = session_container.create_with_session(session, user_id, group_id)
     await ChatCP.finish(f"创建并加入会话 '{new_session.name}' 成功!", at_sender=True)
 
 
 @ChatPrompt.handle()
@@ -254,28 +257,28 @@
     if user_id not in group_usage:
         await ChatWho.finish('当前没有加入任何会话，请加入或创建一个会话')
     session: Session = group_usage[user_id]
     msg = f'当前所在会话信息:\n' \
           f"名称:{session.name[:10]}\n" \
           f"创建者:{session.creator}\n" \
           f"时间:{datetime.fromtimestamp(session.creation_time)}\n" \
-          f"可以使用 /chat dump 导出json字符串格式的上下文信息"
+          f"可以使用 {menu_chat_str} dump 导出json字符串格式的上下文信息"
     await ChatWho.finish(msg)
 
 
 @ChatCopy.handle()
 async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     session_id = int(info.get('id', '').strip())
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     await auth_check(ChatCopy, bot, event, group_id)
     group_sessions: List[Session] = session_container.get_group_sessions(group_id)
     group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if not group_sessions:
-        await ChatCopy.finish("本群尚未创建过会话!请用/chat new命令来创建会话!", at_sender=True)
+        await ChatCopy.finish(f"本群尚未创建过会话!请用{menu_chat_str} new命令来创建会话!", at_sender=True)
     if session_id < 1 or session_id > len(group_sessions):
         await ChatCopy.finish("序号超出!", at_sender=True)
     session: Session = group_sessions[session_id - 1]
     if user_id in group_usage:
         group_usage[user_id].del_user(user_id)
     new_session: Session = session_container.create_with_session(session, user_id, group_id)
     await ChatCopy.finish(f"创建并加入会话 '{new_session.name}' 成功!", at_sender=True)
@@ -316,15 +319,15 @@
 @Join.handle()
 async def _(event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     session_id: int = int(info.get('id', '').strip())
     group_id: str = get_group_id(event)
     group_sessions: List[Session] = session_container.get_group_sessions(group_id)
     group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if not group_sessions:
-        await Join.finish("本群尚未创建过会话!请用/chat new命令来创建会话!", at_sender=True)
+        await Join.finish(f"本群尚未创建过会话!请用{menu_chat_str} new命令来创建会话!", at_sender=True)
     if session_id < 1 or session_id > len(group_sessions):
         await Join.finish("序号超出!", at_sender=True)
     user_id: int = int(event.get_user_id())
     session: Session = group_sessions[session_id - 1]
     if user_id in group_usage:
         group_usage[user_id].del_user(user_id)
     session.add_user(user_id)
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/config.py` & `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py` & `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py` & `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/sessions.py` & `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/sessions.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.6.0
+Version: 1.6.1
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.0/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.6.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.6.0',
+    version='1.6.1',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

