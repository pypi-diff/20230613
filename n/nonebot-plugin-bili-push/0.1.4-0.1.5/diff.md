# Comparing `tmp/nonebot_plugin_bili_push-0.1.4.tar.gz` & `tmp/nonebot_plugin_bili_push-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bili_push-0.1.4.tar", last modified: Tue Jun 13 08:19:27 2023, max compression
+gzip compressed data, was "nonebot_plugin_bili_push-0.1.5.tar", last modified: Tue Jun 13 10:12:07 2023, max compression
```

## Comparing `nonebot_plugin_bili_push-0.1.4.tar` & `nonebot_plugin_bili_push-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:19:27.947170 nonebot_plugin_bili_push-0.1.4/
--rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      268 2023-06-13 08:19:27.947170 nonebot_plugin_bili_push-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2023-06-12 19:01:08.000000 nonebot_plugin_bili_push-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 08:19:27.937167 nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push/
--rw-rw-rw-   0        0        0   101812 2023-06-13 08:18:10.000000 nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:19:27.945167 nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push.egg-info/
--rw-rw-rw-   0        0        0      268 2023-06-13 08:19:27.000000 nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-13 08:19:27.000000 nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 08:19:27.000000 nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-06-13 08:19:27.000000 nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 08:19:27.000000 nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 08:19:27.948168 nonebot_plugin_bili_push-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      794 2023-06-13 08:18:58.000000 nonebot_plugin_bili_push-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:12:07.090541 nonebot_plugin_bili_push-0.1.5/
+-rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      268 2023-06-13 10:12:07.089540 nonebot_plugin_bili_push-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-06-13 09:23:15.000000 nonebot_plugin_bili_push-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 10:12:07.075543 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push/
+-rw-rw-rw-   0        0        0   101668 2023-06-13 10:10:25.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:12:07.087540 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-06-13 10:12:06.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-13 10:12:07.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:12:06.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-06-13 10:12:06.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 10:12:06.000000 nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 10:12:07.090541 nonebot_plugin_bili_push-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-06-13 10:11:37.000000 nonebot_plugin_bili_push-0.1.5/setup.py
```

### Comparing `nonebot_plugin_bili_push-0.1.4/LICENSE` & `nonebot_plugin_bili_push-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-0.1.4/README.md` & `nonebot_plugin_bili_push-0.1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -5,33 +5,46 @@
 </div>
 
 <div align="center">
 
 # nonebot-plugin-bili-push
  B订阅推送插件 
 </div>
+
 ## 示例
 
 ![输入图片描述](README_md_files/9cf89890-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
 ![输入图片描述](README_md_files/7fd7ee50-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
 
 
 ## 安装
-（以下方法二选一）
+（以下方法三选一）
+
+~~一.命令行安装：（未就绪）~~
+
+    nb plugin install nonebot-plugin-bili-push
+ 二.使用插件文件安装：（不推荐）
+ 1.下载插件文件，放到plugins文件夹。
+2.修改pyproject.toml使其可以加载插件
 
-~~命令行安装：（未完成）~~
+三.pip安装：（不推荐）
+1.执行此命令
 
     pip install nonebot-plugin-bili-push
- 使用插件文件安装：
- 下载插件文件，放到plugins文件夹，并修改pyproject.toml使其可以加载插件
-## 配置
+2.修改pyproject.toml使其可以加载插件
 
+    plugins = [”nonebot-plugin-bili-push“]
  
+## 配置
 在 nonebot2 项目的`.env`文件中选填配置
 配置管理员账户，只有管理员才能添加订阅
 
     SUPERUSERS=["12345678"] # 配置 NoneBot 超级用户
 插件数据存放位置，默认为 “./”。
 
     bilipush_basepath="./"
+## 参考内容
+Mirai动态绘制插件 [BilibiliDynamic MiraiPlugin](https://github.com/Colter23/bilibili-dynamic-mirai-plugin)
 
-
+## 交流
+-   交流群[鸽子窝里有鸽子（291788927）](https://qm.qq.com/cgi-bin/qm/qr?k=QhOk7Z2jaXBOnAFfRafEy9g5WoiETQhy&jump_from=webapi&authKey=fCvx/auG+QynlI8bcFNs4Csr2soR8UjzuwLqrDN9F8LDwJrwePKoe89psqpozg/m)
+-   有疑问或者建议都可以进群详谈。
```

#### html2text {}

```diff
@@ -1,13 +1,22 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                 # nonebot-plugin-bili-push Bè®¢éæ¨éæä»¶
 ## ç¤ºä¾ ![è¾å¥å¾çæè¿°](README_md_files/9cf89890-0952-11ee-8733-
 25d9c7397331.jpeg?v=1&type=image) ![è¾å¥å¾çæè¿°](README_md_files/
 7fd7ee50-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image) ## å®è£
-ï¼ä»¥ä¸æ¹æ³äºéä¸ï¼ ~~å½ä»¤è¡å®è£ï¼ï¼æªå®æï¼~~ pip install
-nonebot-plugin-bili-push ä½¿ç¨æä»¶æä»¶å®è£ï¼
-ä¸è½½æä»¶æä»¶ï¼æ¾å°pluginsæä»¶å¤¹ï¼å¹¶ä¿®æ¹pyproject.tomlä½¿å¶å¯ä»¥å è½½æä»¶
-## éç½® å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­éå¡«éç½®
+ï¼ä»¥ä¸æ¹æ³ä¸éä¸ï¼ ~~ä¸.å½ä»¤è¡å®è£ï¼ï¼æªå°±ç»ªï¼~~ nb plugin
+install nonebot-plugin-bili-push äº.ä½¿ç¨æä»¶æä»¶å®è£ï¼ï¼ä¸æ¨èï¼
+1.ä¸è½½æä»¶æä»¶ï¼æ¾å°pluginsæä»¶å¤¹ã
+2.ä¿®æ¹pyproject.tomlä½¿å¶å¯ä»¥å è½½æä»¶ ä¸.pipå®è£ï¼ï¼ä¸æ¨èï¼
+1.æ§è¡æ­¤å½ä»¤ pip install nonebot-plugin-bili-push
+2.ä¿®æ¹pyproject.tomlä½¿å¶å¯ä»¥å è½½æä»¶ plugins = [ânonebot-plugin-
+bili-pushâ] ## éç½® å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­éå¡«éç½®
 éç½®ç®¡çåè´¦æ·ï¼åªæç®¡çåæè½æ·»å è®¢é SUPERUSERS=
 ["12345678"] # éç½® NoneBot è¶çº§ç¨æ· æä»¶æ°æ®å­æ¾ä½ç½®ï¼é»è®¤ä¸º
-â./âã bilipush_basepath="./"
+â./âã bilipush_basepath="./" ## åèåå®¹ Miraiå¨æç»å¶æä»¶
+[BilibiliDynamic MiraiPlugin](https://github.com/Colter23/bilibili-dynamic-
+mirai-plugin) ## äº¤æµ - äº¤æµç¾¤[é¸½å­çªéæé¸½å­ï¼291788927ï¼]
+(https://qm.qq.com/cgi-bin/qm/
+qr?k=QhOk7Z2jaXBOnAFfRafEy9g5WoiETQhy&jump_from=webapi&authKey=fCvx/
+auG+QynlI8bcFNs4Csr2soR8UjzuwLqrDN9F8LDwJrwePKoe89psqpozg/m) -
+æçé®æèå»ºè®®é½å¯ä»¥è¿ç¾¤è¯¦è°ã
```

### Comparing `nonebot_plugin_bili_push-0.1.4/nonebot_plugin_bili_push/__init__.py` & `nonebot_plugin_bili_push-0.1.5/nonebot_plugin_bili_push/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1959,18 +1959,14 @@
                             subscriptionlist.append(uid)
                 else:
                     groupcode = groupcode.removeprefix("g")
                     if groupcode in grouplist:
                         if uid not in subscriptionlist:
                             subscriptionlist.append(uid)
 
-            uids = ["1459104794", "171818544", "354218272"]
-            for uid in uids:
-                subscriptionlist.append(str(uid))
-
             for uid in subscriptionlist:
                 print('-----------------------开始获取信息----------')
                 url = 'https://api.vc.bilibili.com/dynamic_svr/v1/dynamic_svr/space_history?host_uid=' + uid
                 s = json.dumps({'key1': 'value1', 'key2': 'value2'})
                 h = {'Content-Type': 'application/x-www-form-urlencoded'}
                 returnjson = requests.post(url, data=s, headers=h).text
                 returnjson = json.loads(returnjson)
```

### Comparing `nonebot_plugin_bili_push-0.1.4/setup.py` & `nonebot_plugin_bili_push-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         'nonebot_adapter_onebot>=2.2.3',
         'nonebot_plugin_apscheduler>=0.2.0'
     ]
     return reqs
 
 
 setup(name='nonebot_plugin_bili_push',
-      version='0.1.4',
-      description='Nonebot2 plugin',
+      version='0.1.5',
+      description='nonebot2 plugin',
       author='SuperGuGuGu',
       author_email='13680478000@163.com',
       url='https://github.com/SuperGuGuGu/nonebot_plugin_bili_push',
       packages=find_packages(),
       python_requires=">=3.8",
       install_requires=get_install_requires(),
       package_data={'': ['*.csv', '*.txt', '.toml']},
```

