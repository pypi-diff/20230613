# Comparing `tmp/lztmarketapi-0.1.tar.gz` & `tmp/lztmarketapi-0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lztmarketapi-0.1.tar", last modified: Tue Jun 13 03:42:58 2023, max compression
+gzip compressed data, was "lztmarketapi-0.1a0.tar", last modified: Tue Jun 13 03:50:20 2023, max compression
```

## Comparing `lztmarketapi-0.1.tar` & `lztmarketapi-0.1a0.tar`

### file list

```diff
@@ -1,14 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 03:42:58.780990 lztmarketapi-0.1/
--rw-rw-rw-   0        0        0    11558 2023-06-13 03:32:21.000000 lztmarketapi-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      609 2023-06-13 03:42:58.780990 lztmarketapi-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5603 2023-06-13 03:32:21.000000 lztmarketapi-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 03:42:58.773983 lztmarketapi-0.1/lztmarketapi/
--rw-rw-rw-   0        0        0      237 2023-06-13 03:32:21.000000 lztmarketapi-0.1/lztmarketapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:42:58.778982 lztmarketapi-0.1/lztmarketapi.egg-info/
--rw-rw-rw-   0        0        0      609 2023-06-13 03:42:58.000000 lztmarketapi-0.1/lztmarketapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-13 03:42:58.000000 lztmarketapi-0.1/lztmarketapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 03:42:58.000000 lztmarketapi-0.1/lztmarketapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 03:42:58.000000 lztmarketapi-0.1/lztmarketapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 03:42:58.000000 lztmarketapi-0.1/lztmarketapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 03:42:58.781982 lztmarketapi-0.1/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-06-13 03:42:52.000000 lztmarketapi-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.939174 lztmarketapi-0.1a0/
+-rw-rw-rw-   0        0        0    11558 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/LICENSE.txt
+-rw-rw-rw-   0        0        0      611 2023-06-13 03:50:20.940174 lztmarketapi-0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5603 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.885204 lztmarketapi-0.1a0/lztmarketapi/
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.894189 lztmarketapi-0.1a0/lztmarketapi/ApiWrapper/
+-rw-rw-rw-   0        0        0       86 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/ApiWrapper/ApiExceptions.py
+-rw-rw-rw-   0        0        0     3690 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/ApiWrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.895189 lztmarketapi-0.1a0/lztmarketapi/Client/
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.897189 lztmarketapi-0.1a0/lztmarketapi/Client/Games/
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.936176 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/
+-rw-rw-rw-   0        0        0     2101 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/BaseGame.py
+-rw-rw-rw-   0        0        0     1453 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Battlenet.py
+-rw-rw-rw-   0        0        0     1747 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Blitz.py
+-rw-rw-rw-   0        0        0      803 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Cinema.py
+-rw-rw-rw-   0        0        0     1474 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Discord.py
+-rw-rw-rw-   0        0        0      962 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/EpicGames.py
+-rw-rw-rw-   0        0        0     1103 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py
+-rw-rw-rw-   0        0        0     1835 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Fortnite.py
+-rw-rw-rw-   0        0        0     1714 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py
+-rw-rw-rw-   0        0        0     1343 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Instagram.py
+-rw-rw-rw-   0        0        0     1350 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Origin.py
+-rw-rw-rw-   0        0        0      960 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/SocialClub.py
+-rw-rw-rw-   0        0        0     1429 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Spotify.py
+-rw-rw-rw-   0        0        0     4850 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Steam.py
+-rw-rw-rw-   0        0        0     1153 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Supercell.py
+-rw-rw-rw-   0        0        0     1151 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Telegram.py
+-rw-rw-rw-   0        0        0     1481 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/TikTok.py
+-rw-rw-rw-   0        0        0     1162 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Uplay.py
+-rw-rw-rw-   0        0        0     2273 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/VK.py
+-rw-rw-rw-   0        0        0     1441 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/VPN.py
+-rw-rw-rw-   0        0        0     1898 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Valorant.py
+-rw-rw-rw-   0        0        0     1604 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/WarThunder.py
+-rw-rw-rw-   0        0        0     1082 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/Warface.py
+-rw-rw-rw-   0        0        0     1748 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py
+-rw-rw-rw-   0        0        0      798 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/YouTube.py
+-rw-rw-rw-   0        0        0      760 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/GamesModels/__init__.py
+-rw-rw-rw-   0        0        0     1901 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.936176 lztmarketapi-0.1a0/lztmarketapi/Client/Good/
+-rw-rw-rw-   0        0        0     2689 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Good/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.938175 lztmarketapi-0.1a0/lztmarketapi/Client/Me/
+-rw-rw-rw-   0        0        0      369 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Me/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.939174 lztmarketapi-0.1a0/lztmarketapi/Client/Payment/
+-rw-rw-rw-   0        0        0     7001 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/Payment/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/Client/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-06-13 03:32:21.000000 lztmarketapi-0.1a0/lztmarketapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:50:20.892190 lztmarketapi-0.1a0/lztmarketapi.egg-info/
+-rw-rw-rw-   0        0        0      611 2023-06-13 03:50:20.000000 lztmarketapi-0.1a0/lztmarketapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1798 2023-06-13 03:50:20.000000 lztmarketapi-0.1a0/lztmarketapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 03:50:20.000000 lztmarketapi-0.1a0/lztmarketapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 03:50:20.000000 lztmarketapi-0.1a0/lztmarketapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 03:50:20.000000 lztmarketapi-0.1a0/lztmarketapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 03:50:20.940174 lztmarketapi-0.1a0/setup.cfg
+-rw-rw-rw-   0        0        0      911 2023-06-13 03:50:17.000000 lztmarketapi-0.1a0/setup.py
```

### Comparing `lztmarketapi-0.1/LICENSE.txt` & `lztmarketapi-0.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1/PKG-INFO` & `lztmarketapi-0.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lztmarketapi
-Version: 0.1
+Version: 0.1a0
 Summary: Данная библиотека создана для взаимодействия с api lzt.market.
 Home-page: https://github.com/KazariFox/AsyncMarketLztApi
 Author: KazariFox
 Author-email: 
 License: apache-2.0
 Keywords: lzt,lolzteam,lolzteam market,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lztmarketapi-0.1/README.md` & `lztmarketapi-0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1/lztmarketapi.egg-info/PKG-INFO` & `lztmarketapi-0.1a0/lztmarketapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lztmarketapi
-Version: 0.1
+Version: 0.1a0
 Summary: Данная библиотека создана для взаимодействия с api lzt.market.
 Home-page: https://github.com/KazariFox/AsyncMarketLztApi
 Author: KazariFox
 Author-email: 
 License: apache-2.0
 Keywords: lzt,lolzteam,lolzteam market,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lztmarketapi-0.1/setup.py` & `lztmarketapi-0.1a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from distutils.core import setup
+# from distutils.core import setup
+from setuptools import setup, find_packages
 setup(
   name = 'lztmarketapi',        
-  packages = ['lztmarketapi'],  
-  version = '0.1',    
+  packages = find_packages(),
+  include_package_data=True,
+  version = '0.1a',    
   license='apache-2.0',      
   description = 'Данная библиотека создана для взаимодействия с api lzt.market.',   
   author = 'KazariFox',                  
   author_email = '',     
   url = 'https://github.com/KazariFox/AsyncMarketLztApi',   
   keywords = ['lzt', 'lolzteam', 'lolzteam market', 'api'],  
   install_requires=[
```

