# Comparing `tmp/nonebot_plugin_flexperm-0.6.0.tar.gz` & `tmp/nonebot_plugin_flexperm-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_flexperm-0.6.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_flexperm-0.7.0.tar", max compression
```

## Comparing `nonebot_plugin_flexperm-0.6.0.tar` & `nonebot_plugin_flexperm-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1062 2022-12-24 00:55:10.218321 nonebot_plugin_flexperm-0.6.0/LICENSE
--rw-r--r--   0        0        0      321 2022-12-24 00:55:10.233943 nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/__init__.py
--rw-r--r--   0        0        0     8995 2022-12-24 00:55:10.233943 nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/__init__.pyi
--rw-r--r--   0        0        0     1951 2022-12-24 00:55:10.233943 nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/check.py
--rw-r--r--   0        0        0     5481 2022-12-24 01:56:55.058042 nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/cmds.py
--rw-r--r--   0        0        0      235 2022-12-24 01:56:55.010894 nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/config.py
--rw-r--r--   0        0        0    17203 2022-12-24 02:22:27.366749 nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/core.py
--rw-r--r--   0        0        0      147 2022-12-24 00:55:10.233943 nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/defaults.yml
--rw-r--r--   0        0        0    14523 2022-12-24 01:56:55.035796 nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/plugin.py
--rw-r--r--   0        0        0      582 2022-12-24 02:29:13.823582 nonebot_plugin_flexperm-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2365 2022-12-24 01:58:52.945508 nonebot_plugin_flexperm-0.6.0/README.md
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 nonebot_plugin_flexperm-0.6.0/setup.py
--rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 nonebot_plugin_flexperm-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2498 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/README.md
+-rw-r--r--   0        0        0      321 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/__init__.py
+-rw-r--r--   0        0        0     9098 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/__init__.pyi
+-rw-r--r--   0        0        0     2487 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/adapters.py
+-rw-r--r--   0        0        0     2878 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/check.py
+-rw-r--r--   0        0        0     4789 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/cmds.py
+-rw-r--r--   0        0        0      280 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/config.py
+-rw-r--r--   0        0        0    17147 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/core.py
+-rw-r--r--   0        0        0      147 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/defaults.yml
+-rw-r--r--   0        0        0    14822 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/plugin.py
+-rw-r--r--   0        0        0      138 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/util.py
+-rw-r--r--   0        0        0      585 2023-06-13 10:40:58.922277 nonebot_plugin_flexperm-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 nonebot_plugin_flexperm-0.7.0/PKG-INFO
```

### Comparing `nonebot_plugin_flexperm-0.6.0/LICENSE` & `nonebot_plugin_flexperm-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/__init__.pyi` & `nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Union, overload
 
-from nonebot.adapters import Event
+from nonebot.adapters import Bot, Event
 from nonebot.permission import Permission
 
 Designator = Union[Event, str, None]
 
 
 def register(plugin_name: str) -> "PluginHandler":
     """
@@ -44,19 +44,20 @@
         - 否则，在开头添加 插件名+"." 。
 
         :param perm: 权限名，若传入多个权限则须同时满足。
         :param check_root: 如果传入布尔值，则替代之前 self.check_root() 的设定。
         :return: 权限检查器，可以直接传递给 nonebot 事件响应器。
         """
 
-    def has(self, *perm: str, event: Event = None) -> bool:
+    def has(self, *perm: str, bot: Bot = None, event: Event = None) -> bool:
         """
         检查事件是否具有指定权限。会修饰权限名，详见 __call__ 。不会自动检查根权限，无论是否设置 check_root 。
 
         :param perm: 权限名，若传入多个权限则须同时满足。
+        :param bot: 机器人，默认为当前正在处理事件的机器人。
         :param event: 事件，默认为当前正在处理的事件。
         :return: 检查结果。
         """
 
     @overload
     def add_permission(self, perm: str, *,
                        comment: str = None, create_group: bool = True) -> bool: ...
```

### Comparing `nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/cmds.py` & `nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/cmds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,45 @@
 from nonebot import CommandGroup
-from nonebot.adapters import Bot, Message
-from nonebot.adapters.onebot.v11 import MessageEvent
-from nonebot.params import CommandArg, RawCommand, EventMessage
+from nonebot.adapters import Bot, Event, Message
+from nonebot.params import CommandArg, RawCommand
 from nonebot.typing import T_State
 from . import core
 from .plugin import register
 
 P = register('flexperm')
 
-cg = CommandGroup('flexperm', block=True)
+cg = CommandGroup('flexperm', block=True, force_whitespace=True)
 
 
 def h(x):
     return x.handle()
 
 
-async def ensure_command(msg: Message = EventMessage(), raw_cmd: str = RawCommand()):
-    if not msg or not raw_cmd or not all(seg.is_text() for seg in msg):
-        return False
-
-    first_seg = str(msg[0]).lstrip()
-    if not first_seg.startswith(raw_cmd):
-        return False
-    return (len(msg) == 1 and len(first_seg) == len(raw_cmd)  # 无参数
-            or first_seg[len(raw_cmd)].isspace())  # 命令名后有空格
-
-
-@h(cg.command('reload', rule=ensure_command, permission=P('reload')))
-async def _(bot: Bot, event: MessageEvent, arg: Message = CommandArg()):
+@h(cg.command('reload', permission=P('reload')))
+async def _(bot: Bot, event: Event, arg: Message = CommandArg()):
     force = str(arg).strip() == 'force'
     reloaded = core.reload(force)
     if reloaded:
         await bot.send(event, '重新加载权限配置')
     else:
         await bot.send(event, '有未保存的修改，如放弃修改请添加force参数')
 
 
-@h(cg.command('save', rule=ensure_command, permission=P('reload')))
-async def _(bot: Bot, event: MessageEvent):
+@h(cg.command('save', permission=P('reload')))
+async def _(bot: Bot, event: Event):
     success = core.save_all()
     if success:
         await bot.send(event, '已保存权限配置')
     else:
         await bot.send(event, '部分配置保存失败，请检查控制台输出')
 
 
-@h(cg.command('add', rule=ensure_command, permission=P('edit.perm'), state={'add': True}))
-@h(cg.command('remove', rule=ensure_command, permission=P('edit.perm'), state={'add': False}))
-async def _(bot: Bot, event: MessageEvent, state: T_State,
+@h(cg.command('add', permission=P('edit.perm'), state={'add': True}))
+@h(cg.command('remove', permission=P('edit.perm'), state={'add': False}))
+async def _(bot: Bot, event: Event, state: T_State,
             raw_command: str = RawCommand(), arg: Message = CommandArg()):
     args = str(arg).split()
 
     # 一个参数，编辑当前会话的权限
     if len(args) == 1:
         item = args[0]
         designator = event
@@ -79,17 +67,17 @@
     else:
         if result:
             await bot.send(event, '已修改权限组')
         else:
             await bot.send(event, '权限组中{}指定描述'.format('已有' if state['add'] else '没有'))
 
 
-@h(cg.command('addinh', rule=ensure_command, permission=P('edit.inherit'), state={'add': True}))
-@h(cg.command('rminh', rule=ensure_command, permission=P('edit.inherit'), state={'add': False}))
-async def _(bot: Bot, event: MessageEvent, state: T_State,
+@h(cg.command('addinh', permission=P('edit.inherit'), state={'add': True}))
+@h(cg.command('rminh', permission=P('edit.inherit'), state={'add': False}))
+async def _(bot: Bot, event: Event, state: T_State,
             raw_command: str = RawCommand(), arg: Message = CommandArg()):
     args = str(arg).split()
 
     # 一个参数，编辑当前会话的权限
     if len(args) == 1:
         target = args[0]
         designator = event
@@ -113,18 +101,18 @@
     else:
         if result:
             await bot.send(event, '已修改权限组')
         else:
             await bot.send(event, '权限组中{}指定继承关系'.format('已有' if state['add'] else '没有'))
 
 
-@h(cg.command('addgrp', rule=ensure_command, permission=P('edit.group'), state={'add': True}))
-@h(cg.command('rmgrp', rule=ensure_command, permission=P('edit.group'), state={'add': False, 'force': False}))
-@h(cg.command('rmgrpf', rule=ensure_command, permission=P('edit.group.force'), state={'add': False, 'force': True}))
-async def _(bot: Bot, event: MessageEvent, state: T_State,
+@h(cg.command('addgrp', permission=P('edit.group'), state={'add': True}))
+@h(cg.command('rmgrp', permission=P('edit.group'), state={'add': False, 'force': False}))
+@h(cg.command('rmgrpf', permission=P('edit.group.force'), state={'add': False, 'force': True}))
+async def _(bot: Bot, event: Event, state: T_State,
             raw_command: str = RawCommand(), arg: Message = CommandArg()):
     arg = str(arg).strip()
 
     # 无参数，编辑当前会话权限组
     if not arg:
         designator = event
     # 一个参数，编辑指定权限组
```

### Comparing `nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/core.py` & `nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 
 import nonebot
 from nonebot.log import logger
 from pydantic import BaseModel, parse_obj_as
 from ruamel.yaml import YAML, YAMLError, CommentedMap, CommentedSeq
 
 from .config import c
+from .util import try_int
 
 nonebot.require('nonebot_plugin_apscheduler')
 from nonebot_plugin_apscheduler import scheduler
 
 yaml = YAML()
 nonebot_driver = nonebot.get_driver()
 
 loaded: Dict[str, "Namespace"] = {}
 loaded_by_path: Dict[Path, "Namespace"] = {}
 plugin_namespaces: List["Namespace"] = []
 default_groups: Set[str] = set()
 
 
-def get(namespace: str, group: Union[str, int], referer: "PermissionGroup" = None, required: bool = False):
+def get(namespace: str, group: Union[str, int], referer: "PermissionGroup" = None, required: bool = False
+        ) -> "PermissionGroup":
     """
     获取权限组。
 
     :param namespace: 名称空间。
     :param group: 组名。
     :param referer: 引用者。
     :param required: 权限组不存在时是否报错。若存在但有其他问题，则无论该参数设置，都会报错。
-    :return:
-        [0] 权限组，若失败则返回一个空组。 <br>
-        [1] 是否成功。
+    :return: 权限组，若失败则返回一个空组。
     """
     return get_namespace(namespace, required).get_group(group, referer, required)
 
 
 def get_namespace(namespace: str, required: bool, path_override: Path = None) -> "Namespace":
     ns = loaded.get(namespace)
     if ns is None:
@@ -136,88 +136,88 @@
         elif not required and not path.is_file():
             self.config = CommentedMap()
         else:
             try:
                 doc = yaml.load(path)
             except (OSError, YAMLError):
                 logger.exception('Failed to load namespace {} ({})', namespace, path)
-                doc = {}
+                doc = CommentedMap()
 
             if not isinstance(doc, CommentedMap):
                 logger.error('Expect a dict: {} ({})', namespace, path)
-                doc = {}
+                doc = CommentedMap()
 
             self.config: CommentedMap[Union[str, int], dict] = doc
 
     def save(self):
         """
         把本名称空间保存到硬盘上。若没有修改过则不做任何事。
         """
         if self.modifiable and self.dirty:
             self.path.parent.mkdir(parents=True, exist_ok=True)
             yaml.dump(self.config, self.path)
             self.dirty = False
 
     def get_group(self, name: Union[str, int], referer: Optional["PermissionGroup"], required: bool
-                  ) -> Tuple["PermissionGroup", bool]:
+                  ) -> "PermissionGroup":
         """
         获取本名称空间下的权限组。
 
         :param name: 组名。
         :param referer: 引用者。
         :param required: 权限组不存在时是否报错。
         :return:
             [0] 权限组，若失败则返回一个空组。 <br>
             [1] 是否成功。
         """
         group = self.groups.get(name)
         if group is not None:
             if not group.referer:
-                return group, group.namespace is not None
+                return group
 
             cycle = [f'{self.name}:{name}']
             it = referer
             while it and not (it.name == name and it.namespace is self):
                 cycle.append(it.qualified_name())
                 it = it.referer
             cycle.append(f'{self.name}:{name}')
             logger.error('Inheritance cycle detected: {}', ' -> '.join(reversed(cycle)))
-            return NullPermissionGroup(), False
+            return NullPermissionGroup()
 
-        group, found = self._get_group_uncached(name, referer, required)
+        group = self._get_group_uncached(name, referer, required)
         self.groups[name] = group
-        return group, found
+        return group
 
     def _get_group_uncached(self, name: Union[str, int], referer: Optional["PermissionGroup"], required: bool
-                            ) -> Tuple["PermissionGroup", bool]:
+                            ) -> "PermissionGroup":
         group_desc = self.config.get(name)
         if group_desc is None:
             if required:
                 if referer:
                     logger.error('Permission group {}:{} not found (required from {})',
                                  self.name, name, referer.qualified_name())
                 else:
                     logger.error('Permission group {}:{} not found', self.name, name)
-            return NullPermissionGroup(), False
+            return NullPermissionGroup()
 
         try:
             desc = parse_obj_as(GroupDesc, group_desc)
         except ValueError:
             logger.exception('Failed to parse {}:{} ({})', self.name, name, self.path)
-            return NullPermissionGroup(), False
+            return NullPermissionGroup()
 
         # 注入插件预设
         if self.name == 'global' and name in default_groups:
             for pn in plugin_namespaces:
                 if name in pn.config:
                     desc.inherits.append(f'{pn.name}:{name}')
 
         self.groups[name] = group = PermissionGroup(self, name)
         group.populate(desc, referer, self.name if self.auto_decorate else None)
-        return group, True
+        return group
 
     @contextmanager
     def modifying(self, name: Union[str, int] = None):
         if not self.modifiable:
             raise TypeError('Unmodifiable')
         yield self.config[name] if name is not None else None
         self.dirty = True
@@ -259,14 +259,15 @@
 class PermissionGroup:
     """
     权限组。
     """
 
     # 仅在加载过程中有效，加载完成后恢复None。该权限组的引用者，若没有引用者则指向自己。
     referer: Optional["PermissionGroup"] = None
+    is_valid: bool = True
 
     def __init__(self, namespace: Namespace, name: Union[str, int]):
         self.namespace = namespace
         self.name = name
         self.denies: Set[str] = set()
         self.allows: Set[str] = set()
         self.inherits: List[PermissionGroup] = []
@@ -318,16 +319,16 @@
         :param referer: 引用者。
         :param decorate_base: 如果需要修饰，插件名。
         """
         self.referer = referer or self
 
         for parent in desc.inherits:
             namespace, group = parse_qualified_group_name(parent, self.namespace.name)
-            res, found = get(namespace, group, self, True)
-            if found:
+            res = get(namespace, group, self, True)
+            if res.is_valid:
                 self.inherits.append(res)
 
         for item in desc.permissions:
             if item.startswith('-'):
                 target = self.denies
                 item = item[1:]
             else:
@@ -468,16 +469,15 @@
 def parse_qualified_group_name(qn: str, default_namespace: str = 'global') -> Tuple[str, Union[str, int]]:
     split = qn.split(':', maxsplit=1)
     if len(split) == 1:
         namespace, group = default_namespace, split[0]
     else:
         namespace, group = split
     if namespace in ['group', 'user']:
-        with contextlib.suppress(ValueError):
-            group = int(group)
+        group = try_int(group)
     return namespace, group
 
 
 def decorate_permission(base: str, perm: Iterable[str]) -> List[str]:
     result = []
     for p in perm:
         if not p:
@@ -497,14 +497,15 @@
         def __new__(cls, *args, **kwargs):
             raise TypeError
 
 else:
     class NullPermissionGroup:
         referer = None
         namespace = None
+        is_valid = False
 
         def __init__(self):
             pass
 
         def __repr__(self):
             return f'<NullPermissionGroup>'
```

### Comparing `nonebot_plugin_flexperm-0.6.0/nonebot_plugin_flexperm/plugin.py` & `nonebot_plugin_flexperm-0.7.0/nonebot_plugin_flexperm/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
 from pathlib import Path
 from typing import Optional, Dict, Union, Tuple
 
-from nonebot.adapters import Event
+from nonebot.adapters import Bot, Event
 from nonebot.log import logger
-from nonebot.matcher import current_event
+from nonebot.matcher import current_bot, current_event
 from nonebot.permission import Permission
 
 from .check import check, get_permission_group_by_event
 from .core import get, get_namespace, PermissionGroup, decorate_permission, parse_qualified_group_name
 
 plugins: Dict[str, "PluginHandler"] = {}
 
@@ -81,34 +81,37 @@
             check_root = self.check_root_
         if check_root:
             full.insert(0, self.name)
 
         if len(full) == 1:
             single = full[0]
 
-            async def _check(event):
-                return check(event, single)
+            async def _check(bot: Bot, event: Event):
+                return check(bot, event, single)
         else:
-            async def _check(event):
-                return all(check(event, px) for px in full)
+            async def _check(bot: Bot, event: Event):
+                return all(check(bot, event, px) for px in full)
 
         return Permission(_check)
 
-    def has(self, *perm: str, event: Event = None) -> bool:
+    def has(self, *perm: str, bot: Bot = None, event: Event = None) -> bool:
         """
         检查事件是否具有指定权限。会修饰权限名，详见 __call__ 。不会自动检查根权限，无论是否设置 check_root 。
 
         :param perm: 权限名，若传入多个权限则须同时满足。
+        :param bot: 机器人，默认为当前正在处理事件的机器人。
         :param event: 事件，默认为当前正在处理的事件。
         :return: 检查结果。
         """
+        if bot is None or event is None:
+            bot = current_bot.get()
         if event is None:
             event = current_event.get()
         full = decorate_permission(self.name, perm)
-        return all(check(event, px) for px in full)
+        return all(check(bot, event, px) for px in full)
 
     def add_permission(self, designator: Designator, perm: str = _sentinel, *,
                        comment: str = None, create_group: bool = True) -> bool:
         """
         向权限组添加一项权限。会修饰权限名。
 
         实质是移除 perm 的"撤销"权限描述，并添加"授予"权限描述。
@@ -329,28 +332,29 @@
 
     @classmethod
     def _parse_designator(cls, designator: Designator, default_namespace: str = 'global'
                           ) -> Tuple[str, Union[str, int]]:
         if designator is None:
             designator = current_event.get()
         if isinstance(designator, Event):
-            result = get_permission_group_by_event(designator)
+            bot = current_bot.get()
+            result = get_permission_group_by_event(bot, designator)
             if result is not None:
                 return result
             raise ValueError('Unrecognized event type: ' + designator.get_event_name())
         if isinstance(designator, str):
             return parse_qualified_group_name(designator, default_namespace)
         raise ValueError(f'Invalid designator: {type(designator)}')
 
     @classmethod
     def _get_or_create_group(cls, designator: Designator, silent: bool, create: bool, default_namespace: str = 'global'
                              ) -> Optional[PermissionGroup]:
-        namespace, group = cls._parse_designator(designator, default_namespace)
-        group_, found = get(namespace, group)
-        if not found:
+        namespace, group_name = cls._parse_designator(designator, default_namespace)
+        group = get(namespace, group_name)
+        if not group.is_valid:
             if not silent:
                 raise KeyError('No such group')
             if not create:
                 return None
-            get_namespace(namespace, False).add_group(group)
-            group_, _ = get(namespace, group)
-        return group_
+            get_namespace(namespace, False).add_group(group_name)
+            group = get(namespace, group_name)
+        return group
```

### Comparing `nonebot_plugin_flexperm-0.6.0/pyproject.toml` & `nonebot_plugin_flexperm-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-flexperm"
-version = "0.6.0"
+version = "0.7.0"
 description = "精细化的 NoneBot 权限管理插件"
 license = "MIT"
 authors = ["Muchan <liuzh1773@buaa.edu.cn>"]
 readme = "README.md"
 repository = "https://github.com/rmuchan/nonebot-plugin-flexperm"
 keywords = ["nonebot"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = "^2.0.0rc2"
-nonebot-adapter-onebot = "^2.2.0"
+nonebot2 = "^2.0.0"
 "ruamel.yaml" = "^0.17.10"
 nonebot-plugin-apscheduler = "^0.2.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+nonebot-adapter-onebot = "^2.2.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_flexperm-0.6.0/README.md` & `nonebot_plugin_flexperm-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ```shell
 pip install nonebot-plugin-flexperm
 ```
 
 ## 依赖
 
-目前只支持 OneBot V11 协议，之后可能会支持其他协议。
+依赖`nonebot^2.0.0`，支持的协议见[这里](docs/adapters.md)。
 
 ## 使用
 
 本插件主要通过 NoneBot 的 require 机制向**其他插件**提供功能。本插件也提供了一组命令，用于直接管理权限配置。
 
 ```python
 from nonebot import require
@@ -74,16 +74,17 @@
 
 权限配置文件可以在运行时修改，然后使用`/flexperm.reload`命令重新加载。
 
 也可以通过命令编辑权限配置，详见[命令文档](docs/command.md)。
 
 ## 配置
 
-本插件使用2个配置项，均为可选。如需修改，写入 NoneBot 项目环境文件`.env.*`即可。
+本插件使用3个配置项，均为可选。如需修改，写入 NoneBot 项目环境文件`.env.*`即可。
 
 - `flexperm_base`: 权限配置文件所在目录，默认为`permissions`。
 - `flexperm_debug_check`: 是否输出检查权限过程中的调试信息，默认为`false`。未启用 NoneBot 的调试模式时无效。
+- `flexperm_default_adapter`: 检查基于用户ID的权限配置时的默认适配器名，不区分大小写，默认为`onebot`。
 
 ## 鸣谢
 
 - [nonebot / nonebot2](https://github.com/nonebot/nonebot2)
 - [Mrs4s / go-cqhttp](https://github.com/Mrs4s/go-cqhttp)
```

### Comparing `nonebot_plugin_flexperm-0.6.0/PKG-INFO` & `nonebot_plugin_flexperm-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-flexperm
-Version: 0.6.0
+Version: 0.7.0
 Summary: 精细化的 NoneBot 权限管理插件
 Home-page: https://github.com/rmuchan/nonebot-plugin-flexperm
 License: MIT
 Keywords: nonebot
 Author: Muchan
 Author-email: liuzh1773@buaa.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.10,<0.18.0)
 Project-URL: Repository, https://github.com/rmuchan/nonebot-plugin-flexperm
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-flexperm
 
 精细化的 NoneBot 权限管理插件。
@@ -45,15 +44,15 @@
 
 ```shell
 pip install nonebot-plugin-flexperm
 ```
 
 ## 依赖
 
-目前只支持 OneBot V11 协议，之后可能会支持其他协议。
+依赖`nonebot^2.0.0`，支持的协议见[这里](docs/adapters.md)。
 
 ## 使用
 
 本插件主要通过 NoneBot 的 require 机制向**其他插件**提供功能。本插件也提供了一组命令，用于直接管理权限配置。
 
 ```python
 from nonebot import require
@@ -97,17 +96,18 @@
 
 权限配置文件可以在运行时修改，然后使用`/flexperm.reload`命令重新加载。
 
 也可以通过命令编辑权限配置，详见[命令文档](docs/command.md)。
 
 ## 配置
 
-本插件使用2个配置项，均为可选。如需修改，写入 NoneBot 项目环境文件`.env.*`即可。
+本插件使用3个配置项，均为可选。如需修改，写入 NoneBot 项目环境文件`.env.*`即可。
 
 - `flexperm_base`: 权限配置文件所在目录，默认为`permissions`。
 - `flexperm_debug_check`: 是否输出检查权限过程中的调试信息，默认为`false`。未启用 NoneBot 的调试模式时无效。
+- `flexperm_default_adapter`: 检查基于用户ID的权限配置时的默认适配器名，不区分大小写，默认为`onebot`。
 
 ## 鸣谢
 
 - [nonebot / nonebot2](https://github.com/nonebot/nonebot2)
 - [Mrs4s / go-cqhttp](https://github.com/Mrs4s/go-cqhttp)
```

