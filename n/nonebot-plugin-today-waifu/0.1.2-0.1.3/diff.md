# Comparing `tmp/nonebot_plugin_today_waifu-0.1.2.tar.gz` & `tmp/nonebot_plugin_today_waifu-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_today_waifu-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_today_waifu-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_today_waifu-0.1.2.tar` & `nonebot_plugin_today_waifu-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1091 2023-04-01 09:24:29.297752 nonebot_plugin_today_waifu-0.1.2/LICENSE
--rw-r--r--   0        0        0     9712 2023-04-22 09:58:32.530323 nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-01 10:49:28.758563 nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/config.py
--rw-r--r--   0        0        0     5072 2023-04-01 07:20:39.639921 nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/record.py
--rw-r--r--   0        0        0      639 2023-04-22 09:58:32.538447 nonebot_plugin_today_waifu-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5806 2023-04-22 09:58:32.548328 nonebot_plugin_today_waifu-0.1.2/README.md
--rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 nonebot_plugin_today_waifu-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-01 09:24:29.297752 nonebot_plugin_today_waifu-0.1.3/LICENSE
+-rw-r--r--   0        0        0    10037 2023-06-13 18:53:05.119782 nonebot_plugin_today_waifu-0.1.3/nonebot_plugin_today_waifu/__init__.py
+-rw-r--r--   0        0        0     1098 2023-06-13 18:53:05.116786 nonebot_plugin_today_waifu-0.1.3/nonebot_plugin_today_waifu/config.py
+-rw-r--r--   0        0        0     5072 2023-04-01 07:20:39.639921 nonebot_plugin_today_waifu-0.1.3/nonebot_plugin_today_waifu/record.py
+-rw-r--r--   0        0        0      639 2023-06-13 18:56:26.719266 nonebot_plugin_today_waifu-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6230 2023-06-13 18:49:45.389999 nonebot_plugin_today_waifu-0.1.3/README.md
+-rw-r--r--   0        0        0     6955 1970-01-01 00:00:00.000000 nonebot_plugin_today_waifu-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_today_waifu-0.1.2/LICENSE` & `nonebot_plugin_today_waifu-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/__init__.py` & `nonebot_plugin_today_waifu-0.1.3/nonebot_plugin_today_waifu/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 import nonebot
 from nonebot import on_regex
 from nonebot.params import RegexDict
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters import Bot
 from nonebot.adapters.onebot.v11 import GROUP, GroupMessageEvent, ActionFailed, Message
+from nonebot.adapters.onebot.v11.permission import GROUP_OWNER, GROUP_ADMIN
 
 from .config import Config
 from .record import get_group_record, save_group_record, construct_waifu_msg, clear_group_record, \
     construct_change_waifu_msg
 
 __plugin_name__ = '今日老婆'
-__plugin_version__ = '0.1.2'
+__plugin_version__ = '0.1.3'
 __plugin_meta__ = PluginMetadata(
     __plugin_name__,
     "随机抽取群友作为老婆吧！",
     (
         "指令表：\n"
         "▶ 今日老婆\n"
         "  ▷ 范围：群聊\n"
@@ -29,19 +30,19 @@
         "  ▷ 范围：群聊\n"
         "  ▷ 介绍：重新抽取老婆\n"
         "▶ (刷新/重置)今日老婆 | (刷新/重置)自定义别名\n"
         "  ▷ 权限：主人\n"
         "  ▷ 范围：群聊\n"
         "  ▷ 介绍：清空今日本群老婆数据\n"
         "▶ (开启/关闭)换老婆\n"
-        "  ▷ 权限：主人\n"
+        "  ▷ 权限：主人/群主/管理员\n"
         "  ▷ 范围：群聊\n"
         "  ▷ 介绍：开启/关闭本群换老婆功能\n"
         "▶ 设置换老婆次数 <N>\n"
-        "  ▷ 权限：主人\n"
+        "  ▷ 权限：主人/群主/管理员\n"
         "  ▷ 范围：群聊\n"
         "  ▷ 介绍：设置本群换老婆最大次数\n"
         "  ▷ 参数：\n"
         "    ▷ N：指定整数次数"
     ),
     Config,
     {
@@ -54,14 +55,19 @@
 global_config = nonebot.get_driver().config
 waifu_config: Config = Config.parse_obj(global_config.dict())
 
 plugin_aliases: List[str] = waifu_config.today_waifu_aliases
 ban_id: Set[int] = waifu_config.today_waifu_ban_id_list
 default_allow_change_waifu: bool = waifu_config.today_waifu_default_change_waifu
 default_limit_times: int = waifu_config.today_waifu_default_limit_times
+today_waifu_superuser_opt: bool = waifu_config.today_waifu_superuser_opt
+if today_waifu_superuser_opt:
+    permission_opt = SUPERUSER
+else:
+    permission_opt = SUPERUSER | GROUP_OWNER | GROUP_ADMIN
 
 # 正则匹配插件名与别名的字符串
 PatternStr = '|'.join([__plugin_name__, ] + plugin_aliases)
 
 # 响应器主体
 today_waifu = on_regex(
     pattern=rf'^\s*({PatternStr})\s*$',
@@ -87,22 +93,22 @@
     priority=7,
     block=True,
 )
 
 # 设置所在群换老婆最大次数
 today_waifu_set_limit_times = on_regex(
     pattern=rf"^\s*设置换老婆次数(?P<times>\d+)\s*$",
-    permission=SUPERUSER,
+    permission=permission_opt,
     priority=7,
     block=True
 )
 
 today_waifu_set_allow_change = on_regex(
     pattern=rf"^\s*(?P<val>开启换老婆|关闭换老婆)\s*$",
-    permission=SUPERUSER,
+    permission=permission_opt,
     priority=7,
     block=True
 )
 
 
 @today_waifu_set_allow_change.handle()
 async def _(event: GroupMessageEvent, val: Dict[str, Any] = RegexDict()):
```

### Comparing `nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/config.py` & `nonebot_plugin_today_waifu-0.1.3/nonebot_plugin_today_waifu/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 from pydantic import BaseModel, Extra, validator
 
 
 class Config(BaseModel, extra=Extra.ignore):
     today_waifu_ban_id_list: Set[int] = set()
     today_waifu_default_change_waifu: bool = True
-    today_waifu_default_limit_times: int = 3
+    today_waifu_default_limit_times: int = 2
     today_waifu_aliases: List[str] = ['每日老婆', ]
     today_waifu_record_dir: Path = Path(__file__).parent / 'record'
+    today_waifu_superuser_opt: bool = False
 
     @validator('today_waifu_record_dir', pre=True)
     def check_path(cls, v) -> Path:
         return Path(v) if v else Path(__file__).parent / 'record'
 
     @validator('today_waifu_ban_id_list', pre=True)
     def check_ban_id(cls, v: List[int]) -> Set[int]:
```

### Comparing `nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/record.py` & `nonebot_plugin_today_waifu-0.1.3/nonebot_plugin_today_waifu/record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_today_waifu-0.1.2/pyproject.toml` & `nonebot_plugin_today_waifu-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_today_waifu"
-version = "0.1.2"
+version = "0.1.3"
 description = "Nonebot2插件 可以随机抽取群友作为老婆"
 authors = ["glamorgan9826 <glamorgan9826@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/glamorgan9826/nonebot-plugin-today-waifu"
 repository = "https://github.com/glamorgan9826/nonebot-plugin-today-waifu"
```

### Comparing `nonebot_plugin_today_waifu-0.1.2/README.md` & `nonebot_plugin_today_waifu-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -98,48 +98,52 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置，实际上可以都不填写
 
-|               配置项                | 必填  | 类型        |                 默认值                 |                   说明                   |
-|:--------------------------------:|:---:|-----------|:-----------------------------------:|:--------------------------------------:|
-|     TODAY_WAIFU_BAN_ID_LIST      |  否  | List[int] |                 []                  |              列表内的id不会被抽到               |
-| TODAY_WAIFU_DEFAULT_CHANGE_WAIFU |  否  | bool      |                true                 |            是否默认开启换老婆功能，默认开启            |
-| TODAY_WAIFU_DEFAULT_LIMIT_TIMES  |  否  | int       |                  3                  |                允许换老婆次数                 |
-|       TODAY_WAIFU_ALIASES        |  否  | List[str] |              ["每日老婆"]               | 今日老婆插件的别名，允许设置多个，即除了"今日老婆"外，也可以用别名触发指令 |
-|      TODAY_WAIFU_RECORD_DIR      |  否  | str       | "nonebot_plugin_today_waifu/record" |       记录保存路径，默认在插件目录下新建record文件夹       |
+|               配置项                | 必填 | 类型        |                 默认值                 |                   说明                   |
+|:--------------------------------:|:--:|-----------|:-----------------------------------:|:--------------------------------------:|
+|     TODAY_WAIFU_BAN_ID_LIST      | 否  | List[int] |                 []                  |              列表内的id不会被抽到               |
+| TODAY_WAIFU_DEFAULT_CHANGE_WAIFU | 否  | bool      |                true                 |            是否默认开启换老婆功能，默认开启            |
+| TODAY_WAIFU_DEFAULT_LIMIT_TIMES  | 否  | int       |                  2                  |                允许换老婆次数                 |
+|       TODAY_WAIFU_ALIASES        | 否  | List[str] |              ["每日老婆"]               | 今日老婆插件的别名，允许设置多个，即除了"今日老婆"外，也可以用别名触发指令 |
+|      TODAY_WAIFU_RECORD_DIR      | 否  | str       | "nonebot_plugin_today_waifu/record" |       记录保存路径，默认在插件目录下新建record文件夹       |
+|    TODAY_WAIFU_SUPERUSER_OPT     | 否  | bool      |                false                |              是否仅主人可设置换老婆               |
 
     # today-waifu 配置样例
     TODAY_WAIFU_BAN_ID_LIST = [2854196310,123456]
     TODAY_WAIFU_DEFAULT_CHANGE_WAIFU = true
     TODAY_WAIFU_DEFAULT_LIMIT_TIMES = 3
     TODAY_WAIFU_ALIASES = ["每日老婆","我的老婆"]
     # TODAY_WAIFU_RECORD_DIR= "" 一般不需要填写，如果需要请填写绝对路径
 
 ## 🎉 使用
 
 ### 指令表
 
-|            指令            | 权限  | 需要@ | 范围  |                说明                |
-|:------------------------:|:---:|:---:|:---:|:--------------------------------:|
-|        今日老婆/自定义别名        | 群员  |  否  | 群聊  | 随机抽取群友作为老婆，返回头像和昵称。当天已经抽取过回复相同老婆 |
-|           换老婆            | 群员  |  否  | 群聊  |              重新抽取老婆              |
-| (刷新/重置)今日老婆/(刷新/重置)自定义别名 | 主人  |  否  | 群聊  |            清空今日本群老婆数据            |
-|        (开启/关闭)换老婆        | 主人  |  否  | 群聊  |           开启/关闭本群换老婆功能           |
-|         设置换老婆次数n         | 主人  |  否  | 群聊  |         设置本群换老婆最大次数，n为整数         |
+|            指令            |    权限     | 需要@ | 范围 |                说明                |
+|:------------------------:|:---------:|:---:|:--:|:--------------------------------:|
+|        今日老婆/自定义别名        |    群员     |  否  | 群聊 | 随机抽取群友作为老婆，返回头像和昵称。当天已经抽取过回复相同老婆 |
+|           换老婆            |    群员     |  否  | 群聊 |              重新抽取老婆              |
+| (刷新/重置)今日老婆/(刷新/重置)自定义别名 |    主人     |  否  | 群聊 |            清空今日本群老婆数据            |
+|        (开启/关闭)换老婆        | 主人/群主/管理员 |  否  | 群聊 |           开启/关闭本群换老婆功能           |
+|         设置换老婆次数n         | 主人/群主/管理员 |  否  | 群聊 |         设置本群换老婆最大次数，n为整数         |
 
 ### 效果图
 
 暂无
 
 ## ✨其他
 
 - [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
 - [dailywife](https://github.com/SonderXiaoming/dailywife): 本项目的灵感及思路来源。
 - [petpet](https://github.com/noneplugin/nonebot-plugin-petpet): 本项目获取群友头像的功能代码来源。
 
 ## 📋版本历史
+
 - 0.1.0 初始版本
 - 0.1.1 更新metadata及修复一些bug
-- 0.1.2 修复每次关闭换老婆状态无法保存bug
+- 0.1.2 修复每次关闭换老婆状态无法保存bug
+- 0.1.3 修改换老婆次数以及是否开启指令允许群主管理员执行。如果想保持原状仅允许主人执行换老婆相关执行则在配置文件中增加项
+  `TODAY_WAIFU_SUPERUSER_OPT = true`
```

#### html2text {}

```diff
@@ -23,36 +23,41 @@
 pdm add nonebot-plugin-today-waifu   poetry poetry add nonebot-plugin-today-
 waifu   conda conda install nonebot-plugin-today-waifu  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_today_waifu"]  ## âï¸ éç½®
 å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®ï¼å®éä¸å¯ä»¥é½ä¸å¡«å
 | éç½®é¡¹ | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:------------------------
---------:|:---:|-----------|:-----------------------------------:|:------------
---------------------------:| | TODAY_WAIFU_BAN_ID_LIST | å¦ | List[int] | [] |
+--------:|:--:|-----------|:-----------------------------------:|:-------------
+-------------------------:| | TODAY_WAIFU_BAN_ID_LIST | å¦ | List[int] | [] |
 åè¡¨åçidä¸ä¼è¢«æ½å° | | TODAY_WAIFU_DEFAULT_CHANGE_WAIFU | å¦ | bool
 | true | æ¯å¦é»è®¤å¼å¯æ¢èå©åè½ï¼é»è®¤å¼å¯ | |
-TODAY_WAIFU_DEFAULT_LIMIT_TIMES | å¦ | int | 3 | åè®¸æ¢èå©æ¬¡æ° | |
+TODAY_WAIFU_DEFAULT_LIMIT_TIMES | å¦ | int | 2 | åè®¸æ¢èå©æ¬¡æ° | |
 TODAY_WAIFU_ALIASES | å¦ | List[str] | ["æ¯æ¥èå©"] |
 ä»æ¥èå©æä»¶çå«åï¼åè®¸è®¾ç½®å¤ä¸ªï¼å³é¤äº"ä»æ¥èå©"å¤ï¼ä¹å¯ä»¥ç¨å«åè§¦åæä»¤
 | | TODAY_WAIFU_RECORD_DIR | å¦ | str | "nonebot_plugin_today_waifu/record" |
-è®°å½ä¿å­è·¯å¾ï¼é»è®¤å¨æä»¶ç®å½ä¸æ°å»ºrecordæä»¶å¤¹ | # today-
-waifu éç½®æ ·ä¾ TODAY_WAIFU_BAN_ID_LIST = [2854196310,123456]
-TODAY_WAIFU_DEFAULT_CHANGE_WAIFU = true TODAY_WAIFU_DEFAULT_LIMIT_TIMES = 3
-TODAY_WAIFU_ALIASES = ["æ¯æ¥èå©","æçèå©"] # TODAY_WAIFU_RECORD_DIR=
-"" ä¸è¬ä¸éè¦å¡«åï¼å¦æéè¦è¯·å¡«åç»å¯¹è·¯å¾ ## ð ä½¿ç¨ ###
+è®°å½ä¿å­è·¯å¾ï¼é»è®¤å¨æä»¶ç®å½ä¸æ°å»ºrecordæä»¶å¤¹ | |
+TODAY_WAIFU_SUPERUSER_OPT | å¦ | bool | false |
+æ¯å¦ä»ä¸»äººå¯è®¾ç½®æ¢èå© | # today-waifu éç½®æ ·ä¾
+TODAY_WAIFU_BAN_ID_LIST = [2854196310,123456] TODAY_WAIFU_DEFAULT_CHANGE_WAIFU
+= true TODAY_WAIFU_DEFAULT_LIMIT_TIMES = 3 TODAY_WAIFU_ALIASES =
+["æ¯æ¥èå©","æçèå©"] # TODAY_WAIFU_RECORD_DIR= ""
+ä¸è¬ä¸éè¦å¡«åï¼å¦æéè¦è¯·å¡«åç»å¯¹è·¯å¾ ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-------------------
------:|:---:|:---:|:---:|:--------------------------------:| | ä»æ¥èå©/
-èªå®ä¹å«å | ç¾¤å | å¦ | ç¾¤è |
+-----:|:---------:|:---:|:--:|:--------------------------------:| |
+ä»æ¥èå©/èªå®ä¹å«å | ç¾¤å | å¦ | ç¾¤è |
 éæºæ½åç¾¤åä½ä¸ºèå©ï¼è¿åå¤´ååæµç§°ãå½å¤©å·²ç»æ½åè¿åå¤ç¸åèå©
 | | æ¢èå© | ç¾¤å | å¦ | ç¾¤è | éæ°æ½åèå© | | (å·æ°/
 éç½®)ä»æ¥èå©/(å·æ°/éç½®)èªå®ä¹å«å | ä¸»äºº | å¦ | ç¾¤è |
-æ¸ç©ºä»æ¥æ¬ç¾¤èå©æ°æ® | | (å¼å¯/å³é­)æ¢èå© | ä¸»äºº | å¦ |
-ç¾¤è | å¼å¯/å³é­æ¬ç¾¤æ¢èå©åè½ | | è®¾ç½®æ¢èå©æ¬¡æ°n | ä¸»äºº
-| å¦ | ç¾¤è | è®¾ç½®æ¬ç¾¤æ¢èå©æå¤§æ¬¡æ°ï¼nä¸ºæ´æ° | ### ææå¾
-ææ  ## â¨å¶ä» - [Nonebot](https://github.com/nonebot/nonebot2):
+æ¸ç©ºä»æ¥æ¬ç¾¤èå©æ°æ® | | (å¼å¯/å³é­)æ¢èå© | ä¸»äºº/ç¾¤ä¸»/
+ç®¡çå | å¦ | ç¾¤è | å¼å¯/å³é­æ¬ç¾¤æ¢èå©åè½ | |
+è®¾ç½®æ¢èå©æ¬¡æ°n | ä¸»äºº/ç¾¤ä¸»/ç®¡çå | å¦ | ç¾¤è |
+è®¾ç½®æ¬ç¾¤æ¢èå©æå¤§æ¬¡æ°ï¼nä¸ºæ´æ° | ### ææå¾ ææ  ##
+â¨å¶ä» - [Nonebot](https://github.com/nonebot/nonebot2):
 æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã - [dailywife]
 (https://github.com/SonderXiaoming/dailywife):
 æ¬é¡¹ç®ççµæåæè·¯æ¥æºã - [petpet](https://github.com/noneplugin/
 nonebot-plugin-petpet): æ¬é¡¹ç®è·åç¾¤åå¤´åçåè½ä»£ç æ¥æºã ##
 ðçæ¬åå² - 0.1.0 åå§çæ¬ - 0.1.1 æ´æ°metadataåä¿®å¤ä¸äºbug
-- 0.1.2 ä¿®å¤æ¯æ¬¡å³é­æ¢èå©ç¶ææ æ³ä¿å­bug
+- 0.1.2 ä¿®å¤æ¯æ¬¡å³é­æ¢èå©ç¶ææ æ³ä¿å­bug - 0.1.3
+ä¿®æ¹æ¢èå©æ¬¡æ°ä»¥åæ¯å¦å¼å¯æä»¤åè®¸ç¾¤ä¸»ç®¡çåæ§è¡ãå¦ææ³ä¿æåç¶ä»åè®¸ä¸»äººæ§è¡æ¢èå©ç¸å³æ§è¡åå¨éç½®æä»¶ä¸­å¢å é¡¹
+`TODAY_WAIFU_SUPERUSER_OPT = true`
```

### Comparing `nonebot_plugin_today_waifu-0.1.2/PKG-INFO` & `nonebot_plugin_today_waifu-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-today-waifu
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nonebot2插件 可以随机抽取群友作为老婆
 Home-page: https://github.com/glamorgan9826/nonebot-plugin-today-waifu
 License: MIT
 Author: glamorgan9826
 Author-email: glamorgan9826@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -119,48 +119,52 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置，实际上可以都不填写
 
-|               配置项                | 必填  | 类型        |                 默认值                 |                   说明                   |
-|:--------------------------------:|:---:|-----------|:-----------------------------------:|:--------------------------------------:|
-|     TODAY_WAIFU_BAN_ID_LIST      |  否  | List[int] |                 []                  |              列表内的id不会被抽到               |
-| TODAY_WAIFU_DEFAULT_CHANGE_WAIFU |  否  | bool      |                true                 |            是否默认开启换老婆功能，默认开启            |
-| TODAY_WAIFU_DEFAULT_LIMIT_TIMES  |  否  | int       |                  3                  |                允许换老婆次数                 |
-|       TODAY_WAIFU_ALIASES        |  否  | List[str] |              ["每日老婆"]               | 今日老婆插件的别名，允许设置多个，即除了"今日老婆"外，也可以用别名触发指令 |
-|      TODAY_WAIFU_RECORD_DIR      |  否  | str       | "nonebot_plugin_today_waifu/record" |       记录保存路径，默认在插件目录下新建record文件夹       |
+|               配置项                | 必填 | 类型        |                 默认值                 |                   说明                   |
+|:--------------------------------:|:--:|-----------|:-----------------------------------:|:--------------------------------------:|
+|     TODAY_WAIFU_BAN_ID_LIST      | 否  | List[int] |                 []                  |              列表内的id不会被抽到               |
+| TODAY_WAIFU_DEFAULT_CHANGE_WAIFU | 否  | bool      |                true                 |            是否默认开启换老婆功能，默认开启            |
+| TODAY_WAIFU_DEFAULT_LIMIT_TIMES  | 否  | int       |                  2                  |                允许换老婆次数                 |
+|       TODAY_WAIFU_ALIASES        | 否  | List[str] |              ["每日老婆"]               | 今日老婆插件的别名，允许设置多个，即除了"今日老婆"外，也可以用别名触发指令 |
+|      TODAY_WAIFU_RECORD_DIR      | 否  | str       | "nonebot_plugin_today_waifu/record" |       记录保存路径，默认在插件目录下新建record文件夹       |
+|    TODAY_WAIFU_SUPERUSER_OPT     | 否  | bool      |                false                |              是否仅主人可设置换老婆               |
 
     # today-waifu 配置样例
     TODAY_WAIFU_BAN_ID_LIST = [2854196310,123456]
     TODAY_WAIFU_DEFAULT_CHANGE_WAIFU = true
     TODAY_WAIFU_DEFAULT_LIMIT_TIMES = 3
     TODAY_WAIFU_ALIASES = ["每日老婆","我的老婆"]
     # TODAY_WAIFU_RECORD_DIR= "" 一般不需要填写，如果需要请填写绝对路径
 
 ## 🎉 使用
 
 ### 指令表
 
-|            指令            | 权限  | 需要@ | 范围  |                说明                |
-|:------------------------:|:---:|:---:|:---:|:--------------------------------:|
-|        今日老婆/自定义别名        | 群员  |  否  | 群聊  | 随机抽取群友作为老婆，返回头像和昵称。当天已经抽取过回复相同老婆 |
-|           换老婆            | 群员  |  否  | 群聊  |              重新抽取老婆              |
-| (刷新/重置)今日老婆/(刷新/重置)自定义别名 | 主人  |  否  | 群聊  |            清空今日本群老婆数据            |
-|        (开启/关闭)换老婆        | 主人  |  否  | 群聊  |           开启/关闭本群换老婆功能           |
-|         设置换老婆次数n         | 主人  |  否  | 群聊  |         设置本群换老婆最大次数，n为整数         |
+|            指令            |    权限     | 需要@ | 范围 |                说明                |
+|:------------------------:|:---------:|:---:|:--:|:--------------------------------:|
+|        今日老婆/自定义别名        |    群员     |  否  | 群聊 | 随机抽取群友作为老婆，返回头像和昵称。当天已经抽取过回复相同老婆 |
+|           换老婆            |    群员     |  否  | 群聊 |              重新抽取老婆              |
+| (刷新/重置)今日老婆/(刷新/重置)自定义别名 |    主人     |  否  | 群聊 |            清空今日本群老婆数据            |
+|        (开启/关闭)换老婆        | 主人/群主/管理员 |  否  | 群聊 |           开启/关闭本群换老婆功能           |
+|         设置换老婆次数n         | 主人/群主/管理员 |  否  | 群聊 |         设置本群换老婆最大次数，n为整数         |
 
 ### 效果图
 
 暂无
 
 ## ✨其他
 
 - [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
 - [dailywife](https://github.com/SonderXiaoming/dailywife): 本项目的灵感及思路来源。
 - [petpet](https://github.com/noneplugin/nonebot-plugin-petpet): 本项目获取群友头像的功能代码来源。
 
 ## 📋版本历史
+
 - 0.1.0 初始版本
 - 0.1.1 更新metadata及修复一些bug
 - 0.1.2 修复每次关闭换老婆状态无法保存bug
+- 0.1.3 修改换老婆次数以及是否开启指令允许群主管理员执行。如果想保持原状仅允许主人执行换老婆相关执行则在配置文件中增加项
+  `TODAY_WAIFU_SUPERUSER_OPT = true`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-today-waifu Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-today-waifu Version: 0.1.3 Summary:
 Nonebot2æä»¶ å¯ä»¥éæºæ½åç¾¤åä½ä¸ºèå© Home-page: https://
 github.com/glamorgan9826/nonebot-plugin-today-waifu License: MIT Author:
 glamorgan9826 Author-email: glamorgan9826@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -35,36 +35,41 @@
 pdm add nonebot-plugin-today-waifu   poetry poetry add nonebot-plugin-today-
 waifu   conda conda install nonebot-plugin-today-waifu  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_today_waifu"]  ## âï¸ éç½®
 å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®ï¼å®éä¸å¯ä»¥é½ä¸å¡«å
 | éç½®é¡¹ | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:------------------------
---------:|:---:|-----------|:-----------------------------------:|:------------
---------------------------:| | TODAY_WAIFU_BAN_ID_LIST | å¦ | List[int] | [] |
+--------:|:--:|-----------|:-----------------------------------:|:-------------
+-------------------------:| | TODAY_WAIFU_BAN_ID_LIST | å¦ | List[int] | [] |
 åè¡¨åçidä¸ä¼è¢«æ½å° | | TODAY_WAIFU_DEFAULT_CHANGE_WAIFU | å¦ | bool
 | true | æ¯å¦é»è®¤å¼å¯æ¢èå©åè½ï¼é»è®¤å¼å¯ | |
-TODAY_WAIFU_DEFAULT_LIMIT_TIMES | å¦ | int | 3 | åè®¸æ¢èå©æ¬¡æ° | |
+TODAY_WAIFU_DEFAULT_LIMIT_TIMES | å¦ | int | 2 | åè®¸æ¢èå©æ¬¡æ° | |
 TODAY_WAIFU_ALIASES | å¦ | List[str] | ["æ¯æ¥èå©"] |
 ä»æ¥èå©æä»¶çå«åï¼åè®¸è®¾ç½®å¤ä¸ªï¼å³é¤äº"ä»æ¥èå©"å¤ï¼ä¹å¯ä»¥ç¨å«åè§¦åæä»¤
 | | TODAY_WAIFU_RECORD_DIR | å¦ | str | "nonebot_plugin_today_waifu/record" |
-è®°å½ä¿å­è·¯å¾ï¼é»è®¤å¨æä»¶ç®å½ä¸æ°å»ºrecordæä»¶å¤¹ | # today-
-waifu éç½®æ ·ä¾ TODAY_WAIFU_BAN_ID_LIST = [2854196310,123456]
-TODAY_WAIFU_DEFAULT_CHANGE_WAIFU = true TODAY_WAIFU_DEFAULT_LIMIT_TIMES = 3
-TODAY_WAIFU_ALIASES = ["æ¯æ¥èå©","æçèå©"] # TODAY_WAIFU_RECORD_DIR=
-"" ä¸è¬ä¸éè¦å¡«åï¼å¦æéè¦è¯·å¡«åç»å¯¹è·¯å¾ ## ð ä½¿ç¨ ###
+è®°å½ä¿å­è·¯å¾ï¼é»è®¤å¨æä»¶ç®å½ä¸æ°å»ºrecordæä»¶å¤¹ | |
+TODAY_WAIFU_SUPERUSER_OPT | å¦ | bool | false |
+æ¯å¦ä»ä¸»äººå¯è®¾ç½®æ¢èå© | # today-waifu éç½®æ ·ä¾
+TODAY_WAIFU_BAN_ID_LIST = [2854196310,123456] TODAY_WAIFU_DEFAULT_CHANGE_WAIFU
+= true TODAY_WAIFU_DEFAULT_LIMIT_TIMES = 3 TODAY_WAIFU_ALIASES =
+["æ¯æ¥èå©","æçèå©"] # TODAY_WAIFU_RECORD_DIR= ""
+ä¸è¬ä¸éè¦å¡«åï¼å¦æéè¦è¯·å¡«åç»å¯¹è·¯å¾ ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-------------------
------:|:---:|:---:|:---:|:--------------------------------:| | ä»æ¥èå©/
-èªå®ä¹å«å | ç¾¤å | å¦ | ç¾¤è |
+-----:|:---------:|:---:|:--:|:--------------------------------:| |
+ä»æ¥èå©/èªå®ä¹å«å | ç¾¤å | å¦ | ç¾¤è |
 éæºæ½åç¾¤åä½ä¸ºèå©ï¼è¿åå¤´ååæµç§°ãå½å¤©å·²ç»æ½åè¿åå¤ç¸åèå©
 | | æ¢èå© | ç¾¤å | å¦ | ç¾¤è | éæ°æ½åèå© | | (å·æ°/
 éç½®)ä»æ¥èå©/(å·æ°/éç½®)èªå®ä¹å«å | ä¸»äºº | å¦ | ç¾¤è |
-æ¸ç©ºä»æ¥æ¬ç¾¤èå©æ°æ® | | (å¼å¯/å³é­)æ¢èå© | ä¸»äºº | å¦ |
-ç¾¤è | å¼å¯/å³é­æ¬ç¾¤æ¢èå©åè½ | | è®¾ç½®æ¢èå©æ¬¡æ°n | ä¸»äºº
-| å¦ | ç¾¤è | è®¾ç½®æ¬ç¾¤æ¢èå©æå¤§æ¬¡æ°ï¼nä¸ºæ´æ° | ### ææå¾
-ææ  ## â¨å¶ä» - [Nonebot](https://github.com/nonebot/nonebot2):
+æ¸ç©ºä»æ¥æ¬ç¾¤èå©æ°æ® | | (å¼å¯/å³é­)æ¢èå© | ä¸»äºº/ç¾¤ä¸»/
+ç®¡çå | å¦ | ç¾¤è | å¼å¯/å³é­æ¬ç¾¤æ¢èå©åè½ | |
+è®¾ç½®æ¢èå©æ¬¡æ°n | ä¸»äºº/ç¾¤ä¸»/ç®¡çå | å¦ | ç¾¤è |
+è®¾ç½®æ¬ç¾¤æ¢èå©æå¤§æ¬¡æ°ï¼nä¸ºæ´æ° | ### ææå¾ ææ  ##
+â¨å¶ä» - [Nonebot](https://github.com/nonebot/nonebot2):
 æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã - [dailywife]
 (https://github.com/SonderXiaoming/dailywife):
 æ¬é¡¹ç®ççµæåæè·¯æ¥æºã - [petpet](https://github.com/noneplugin/
 nonebot-plugin-petpet): æ¬é¡¹ç®è·åç¾¤åå¤´åçåè½ä»£ç æ¥æºã ##
 ðçæ¬åå² - 0.1.0 åå§çæ¬ - 0.1.1 æ´æ°metadataåä¿®å¤ä¸äºbug
-- 0.1.2 ä¿®å¤æ¯æ¬¡å³é­æ¢èå©ç¶ææ æ³ä¿å­bug
+- 0.1.2 ä¿®å¤æ¯æ¬¡å³é­æ¢èå©ç¶ææ æ³ä¿å­bug - 0.1.3
+ä¿®æ¹æ¢èå©æ¬¡æ°ä»¥åæ¯å¦å¼å¯æä»¤åè®¸ç¾¤ä¸»ç®¡çåæ§è¡ãå¦ææ³ä¿æåç¶ä»åè®¸ä¸»äººæ§è¡æ¢èå©ç¸å³æ§è¡åå¨éç½®æä»¶ä¸­å¢å é¡¹
+`TODAY_WAIFU_SUPERUSER_OPT = true`
```

