# Comparing `tmp/nonebot-plugin-warthunder-player-check-0.1.1.tar.gz` & `tmp/nonebot-plugin-warthunder-player-check-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-warthunder-player-check-0.1.1.tar", last modified: Tue Jun 13 17:06:43 2023, max compression
+gzip compressed data, was "nonebot-plugin-warthunder-player-check-0.1.2.tar", last modified: Tue Jun 13 17:17:56 2023, max compression
```

## Comparing `nonebot-plugin-warthunder-player-check-0.1.1.tar` & `nonebot-plugin-warthunder-player-check-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:06:43.914140 nonebot-plugin-warthunder-player-check-0.1.1/
--rw-rw-rw-   0        0        0     1781 2023-06-13 17:06:43.914140 nonebot-plugin-warthunder-player-check-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2023-06-13 16:37:37.000000 nonebot-plugin-warthunder-player-check-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 17:06:43.908566 nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check/
--rw-rw-rw-   0        0        0     6394 2023-06-13 17:05:46.000000 nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:06:43.913140 nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check.egg-info/
--rw-rw-rw-   0        0        0     1781 2023-06-13 17:06:43.000000 nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-13 17:06:43.000000 nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:06:43.000000 nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-06-13 17:06:43.000000 nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check.egg-info/requires.txt
--rw-rw-rw-   0        0        0       39 2023-06-13 17:06:43.000000 nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 17:06:43.914140 nonebot-plugin-warthunder-player-check-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-06-13 17:06:41.000000 nonebot-plugin-warthunder-player-check-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:56.204848 nonebot-plugin-warthunder-player-check-0.1.2/
+-rw-rw-rw-   0        0        0     1781 2023-06-13 17:17:56.204848 nonebot-plugin-warthunder-player-check-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1403 2023-06-13 16:37:37.000000 nonebot-plugin-warthunder-player-check-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:56.198848 nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check/
+-rw-rw-rw-   0        0        0     6392 2023-06-13 17:14:36.000000 nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:56.203868 nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check.egg-info/
+-rw-rw-rw-   0        0        0     1781 2023-06-13 17:17:56.000000 nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-13 17:17:56.000000 nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:17:56.000000 nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-06-13 17:17:56.000000 nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2023-06-13 17:17:56.000000 nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:17:56.205848 nonebot-plugin-warthunder-player-check-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-06-13 17:14:36.000000 nonebot-plugin-warthunder-player-check-0.1.2/setup.py
```

### Comparing `nonebot-plugin-warthunder-player-check-0.1.1/PKG-INFO` & `nonebot-plugin-warthunder-player-check-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-warthunder-player-check
-Version: 0.1.1
+Version: 0.1.2
 Summary: nonebot2 plugin
 Home-page: https://github.com/0Neptune0/nonebot-plugin-warthunder-player-check
 Author: 00.Neptune.00
 Author-email: neptune.0@qq.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot-plugin-warthunder-player-check Version:
-0.1.1 Summary: nonebot2 plugin Home-page: https://github.com/0Neptune0/nonebot-
+0.1.2 Summary: nonebot2 plugin Home-page: https://github.com/0Neptune0/nonebot-
 plugin-warthunder-player-check Author: 00.Neptune.00 Author-email:
 neptune.0@qq.com License: GNU General Public License v3.0 Platform: UNKNOWN
 Requires-Python: >=3.8 Description-Content-Type: text/markdown
                                    [nonebot]
                  # nonebot-plugin-warthunder-player-check _â¨
      Warthunderç©å®¶æç»©æ¥è¯¢æä»¶ â¨_ [license] [nonebot] [release]
 ## ç®ä»
```

### Comparing `nonebot-plugin-warthunder-player-check-0.1.1/README.md` & `nonebot-plugin-warthunder-player-check-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check/__init__.py` & `nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 img_path = str(os.getcwd()).replace('\\', '/') + '/src/plugins/pluto/_cache'
 
 
 __plugin_meta__ = PluginMetadata(
     name='战雷查水表',
     description='搜索warthunder社区查询玩家履历',
     usage='/战雷查水表 [玩家id]',
-    type='`application`',
+    type='application',
     homepage='https://github.com/0Neptune0/nonebot-plugin-warthunder-player-check',
     supported_adapters={'~onebot.v11'}
 )
 
 
 options = Options()
 options.add_argument('--headless')
```

### Comparing `nonebot-plugin-warthunder-player-check-0.1.1/nonebot_plugin_warthunder_player_check.egg-info/PKG-INFO` & `nonebot-plugin-warthunder-player-check-0.1.2/nonebot_plugin_warthunder_player_check.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-warthunder-player-check
-Version: 0.1.1
+Version: 0.1.2
 Summary: nonebot2 plugin
 Home-page: https://github.com/0Neptune0/nonebot-plugin-warthunder-player-check
 Author: 00.Neptune.00
 Author-email: neptune.0@qq.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot-plugin-warthunder-player-check Version:
-0.1.1 Summary: nonebot2 plugin Home-page: https://github.com/0Neptune0/nonebot-
+0.1.2 Summary: nonebot2 plugin Home-page: https://github.com/0Neptune0/nonebot-
 plugin-warthunder-player-check Author: 00.Neptune.00 Author-email:
 neptune.0@qq.com License: GNU General Public License v3.0 Platform: UNKNOWN
 Requires-Python: >=3.8 Description-Content-Type: text/markdown
                                    [nonebot]
                  # nonebot-plugin-warthunder-player-check _â¨
      Warthunderç©å®¶æç»©æ¥è¯¢æä»¶ â¨_ [license] [nonebot] [release]
 ## ç®ä»
```

### Comparing `nonebot-plugin-warthunder-player-check-0.1.1/setup.py` & `nonebot-plugin-warthunder-player-check-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding="utf-8") as md:
     long_description = md.read()
 
 setup(
     name='nonebot-plugin-warthunder-player-check',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "nonebot2 >= 2.0.0",
         "nonebot_adapter_onebot >= 2.2.3",
```

