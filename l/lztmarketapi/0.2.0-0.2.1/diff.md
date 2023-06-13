# Comparing `tmp/lztmarketapi-0.2.0.tar.gz` & `tmp/lztmarketapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lztmarketapi-0.2.0.tar", last modified: Tue Jun 13 03:59:42 2023, max compression
+gzip compressed data, was "lztmarketapi-0.2.1.tar", last modified: Tue Jun 13 04:05:58 2023, max compression
```

## Comparing `lztmarketapi-0.2.0.tar` & `lztmarketapi-0.2.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.236247 lztmarketapi-0.2.0/
--rw-rw-rw-   0        0        0    11558 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      611 2023-06-13 03:59:42.236247 lztmarketapi-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5603 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.142279 lztmarketapi-0.2.0/lztmarketapi/
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.152275 lztmarketapi-0.2.0/lztmarketapi/ApiWrapper/
--rw-rw-rw-   0        0        0       86 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/ApiWrapper/ApiExceptions.py
--rw-rw-rw-   0        0        0     3690 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/ApiWrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.154274 lztmarketapi-0.2.0/lztmarketapi/Client/
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.155274 lztmarketapi-0.2.0/lztmarketapi/Client/Games/
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.205257 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/
--rw-rw-rw-   0        0        0     2101 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/BaseGame.py
--rw-rw-rw-   0        0        0     1453 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Battlenet.py
--rw-rw-rw-   0        0        0     1747 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Blitz.py
--rw-rw-rw-   0        0        0      803 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Cinema.py
--rw-rw-rw-   0        0        0     1474 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Discord.py
--rw-rw-rw-   0        0        0      962 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/EpicGames.py
--rw-rw-rw-   0        0        0     1103 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py
--rw-rw-rw-   0        0        0     1835 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Fortnite.py
--rw-rw-rw-   0        0        0     1714 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py
--rw-rw-rw-   0        0        0     1343 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Instagram.py
--rw-rw-rw-   0        0        0     1350 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Origin.py
--rw-rw-rw-   0        0        0      960 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/SocialClub.py
--rw-rw-rw-   0        0        0     1429 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Spotify.py
--rw-rw-rw-   0        0        0     4850 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Steam.py
--rw-rw-rw-   0        0        0     1153 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Supercell.py
--rw-rw-rw-   0        0        0     1151 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Telegram.py
--rw-rw-rw-   0        0        0     1481 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/TikTok.py
--rw-rw-rw-   0        0        0     1162 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Uplay.py
--rw-rw-rw-   0        0        0     2273 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/VK.py
--rw-rw-rw-   0        0        0     1441 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/VPN.py
--rw-rw-rw-   0        0        0     1898 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Valorant.py
--rw-rw-rw-   0        0        0     1604 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/WarThunder.py
--rw-rw-rw-   0        0        0     1082 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Warface.py
--rw-rw-rw-   0        0        0     1748 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py
--rw-rw-rw-   0        0        0      798 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/YouTube.py
--rw-rw-rw-   0        0        0      760 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/__init__.py
--rw-rw-rw-   0        0        0     1901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.206258 lztmarketapi-0.2.0/lztmarketapi/Client/Good/
--rw-rw-rw-   0        0        0     2689 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Good/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.207257 lztmarketapi-0.2.0/lztmarketapi/Client/Me/
--rw-rw-rw-   0        0        0      369 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Me/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.208257 lztmarketapi-0.2.0/lztmarketapi/Client/Payment/
--rw-rw-rw-   0        0        0     7001 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Payment/__init__.py
--rw-rw-rw-   0        0        0      495 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.230250 lztmarketapi-0.2.0/lztmarketapi/Types/
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.232248 lztmarketapi-0.2.0/lztmarketapi/Types/AccountManage/
--rw-rw-rw-   0        0        0      134 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/AccountManage/ManageExceptions.py
--rw-rw-rw-   0        0        0    15293 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/AccountManage/__init__.py
--rw-rw-rw-   0        0        0     1229 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Category.py
--rw-rw-rw-   0        0        0      106 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Currency.py
--rw-rw-rw-   0        0        0     6474 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Good.py
--rw-rw-rw-   0        0        0       36 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Guarantee.py
--rw-rw-rw-   0        0        0      141 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/ItemOrigin.py
--rw-rw-rw-   0        0        0       38 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Mail.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.233250 lztmarketapi-0.2.0/lztmarketapi/Types/PaymentModel/
--rw-rw-rw-   0        0        0      901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/PaymentModel/__init__.py
--rw-rw-rw-   0        0        0      279 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/PaymentType.py
--rw-rw-rw-   0        0        0      724 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Profile.py
--rw-rw-rw-   0        0        0       21 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Result.py
--rw-rw-rw-   0        0        0       75 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/TimeValues.py
--rw-rw-rw-   0        0        0      349 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/User.py
--rw-rw-rw-   0        0        0       15 2023-06-13 03:58:47.000000 lztmarketapi-0.2.0/lztmarketapi/Types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.235248 lztmarketapi-0.2.0/lztmarketapi/Utils/
--rw-rw-rw-   0        0        0      906 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Utils/Response.py
--rw-rw-rw-   0        0        0       15 2023-06-13 03:59:13.000000 lztmarketapi-0.2.0/lztmarketapi/Utils/__init__.py
--rw-rw-rw-   0        0        0      299 2023-06-13 03:57:53.000000 lztmarketapi-0.2.0/lztmarketapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.149276 lztmarketapi-0.2.0/lztmarketapi.egg-info/
--rw-rw-rw-   0        0        0      611 2023-06-13 03:59:41.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2367 2023-06-13 03:59:42.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 03:59:41.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 03:59:41.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 03:59:41.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 03:59:42.237247 lztmarketapi-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-06-13 03:56:29.000000 lztmarketapi-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.619120 lztmarketapi-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      611 2023-06-13 04:05:58.619120 lztmarketapi-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5603 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.535094 lztmarketapi-0.2.1/lztmarketapi/
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.542463 lztmarketapi-0.2.1/lztmarketapi/ApiWrapper/
+-rw-rw-rw-   0        0        0       86 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/ApiWrapper/ApiExceptions.py
+-rw-rw-rw-   0        0        0     3690 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/ApiWrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.543463 lztmarketapi-0.2.1/lztmarketapi/Client/
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.545464 lztmarketapi-0.2.1/lztmarketapi/Client/Games/
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.583131 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/
+-rw-rw-rw-   0        0        0     2101 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/BaseGame.py
+-rw-rw-rw-   0        0        0     1421 2023-06-13 04:05:15.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Battlenet.py
+-rw-rw-rw-   0        0        0     1715 2023-06-13 04:05:14.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Blitz.py
+-rw-rw-rw-   0        0        0      771 2023-06-13 04:05:13.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Cinema.py
+-rw-rw-rw-   0        0        0     1442 2023-06-13 04:05:13.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Discord.py
+-rw-rw-rw-   0        0        0      930 2023-06-13 04:05:13.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/EpicGames.py
+-rw-rw-rw-   0        0        0     1071 2023-06-13 04:05:12.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py
+-rw-rw-rw-   0        0        0     1803 2023-06-13 04:05:12.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Fortnite.py
+-rw-rw-rw-   0        0        0     1682 2023-06-13 04:05:12.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py
+-rw-rw-rw-   0        0        0     1311 2023-06-13 04:05:11.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Instagram.py
+-rw-rw-rw-   0        0        0     1318 2023-06-13 04:05:11.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Origin.py
+-rw-rw-rw-   0        0        0      928 2023-06-13 04:05:10.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/SocialClub.py
+-rw-rw-rw-   0        0        0     1397 2023-06-13 04:05:10.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Spotify.py
+-rw-rw-rw-   0        0        0     4850 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Steam.py
+-rw-rw-rw-   0        0        0     1121 2023-06-13 04:05:09.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Supercell.py
+-rw-rw-rw-   0        0        0     1119 2023-06-13 04:05:09.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Telegram.py
+-rw-rw-rw-   0        0        0     1449 2023-06-13 04:05:09.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/TikTok.py
+-rw-rw-rw-   0        0        0     1130 2023-06-13 04:05:08.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Uplay.py
+-rw-rw-rw-   0        0        0     2239 2023-06-13 04:03:55.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/VK.py
+-rw-rw-rw-   0        0        0     1409 2023-06-13 04:05:06.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/VPN.py
+-rw-rw-rw-   0        0        0     1868 2023-06-13 04:05:08.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Valorant.py
+-rw-rw-rw-   0        0        0     1572 2023-06-13 04:05:05.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/WarThunder.py
+-rw-rw-rw-   0        0        0     1050 2023-06-13 04:05:06.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Warface.py
+-rw-rw-rw-   0        0        0     1716 2023-06-13 04:05:06.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py
+-rw-rw-rw-   0        0        0      766 2023-06-13 04:05:05.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/YouTube.py
+-rw-rw-rw-   0        0        0      760 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/__init__.py
+-rw-rw-rw-   0        0        0     1901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.584131 lztmarketapi-0.2.1/lztmarketapi/Client/Good/
+-rw-rw-rw-   0        0        0     2689 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Good/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.586130 lztmarketapi-0.2.1/lztmarketapi/Client/Me/
+-rw-rw-rw-   0        0        0      369 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Me/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.587131 lztmarketapi-0.2.1/lztmarketapi/Client/Payment/
+-rw-rw-rw-   0        0        0     7001 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Client/Payment/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.599126 lztmarketapi-0.2.1/lztmarketapi/Types/
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.604126 lztmarketapi-0.2.1/lztmarketapi/Types/AccountManage/
+-rw-rw-rw-   0        0        0      134 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/AccountManage/ManageExceptions.py
+-rw-rw-rw-   0        0        0    15293 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/AccountManage/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/Category.py
+-rw-rw-rw-   0        0        0      106 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/Currency.py
+-rw-rw-rw-   0        0        0     6474 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/Good.py
+-rw-rw-rw-   0        0        0       36 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/Guarantee.py
+-rw-rw-rw-   0        0        0      141 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/ItemOrigin.py
+-rw-rw-rw-   0        0        0       38 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/Mail.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.609123 lztmarketapi-0.2.1/lztmarketapi/Types/PaymentModel/
+-rw-rw-rw-   0        0        0      901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/PaymentModel/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/PaymentType.py
+-rw-rw-rw-   0        0        0      724 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/Profile.py
+-rw-rw-rw-   0        0        0       21 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/Result.py
+-rw-rw-rw-   0        0        0       75 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/TimeValues.py
+-rw-rw-rw-   0        0        0      349 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Types/User.py
+-rw-rw-rw-   0        0        0       15 2023-06-13 03:58:47.000000 lztmarketapi-0.2.1/lztmarketapi/Types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.617120 lztmarketapi-0.2.1/lztmarketapi/Utils/
+-rw-rw-rw-   0        0        0      906 2023-06-13 03:32:21.000000 lztmarketapi-0.2.1/lztmarketapi/Utils/Response.py
+-rw-rw-rw-   0        0        0       15 2023-06-13 03:59:13.000000 lztmarketapi-0.2.1/lztmarketapi/Utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-06-13 03:57:53.000000 lztmarketapi-0.2.1/lztmarketapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:05:58.540464 lztmarketapi-0.2.1/lztmarketapi.egg-info/
+-rw-rw-rw-   0        0        0      611 2023-06-13 04:05:58.000000 lztmarketapi-0.2.1/lztmarketapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2367 2023-06-13 04:05:58.000000 lztmarketapi-0.2.1/lztmarketapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 04:05:58.000000 lztmarketapi-0.2.1/lztmarketapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 04:05:58.000000 lztmarketapi-0.2.1/lztmarketapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 04:05:58.000000 lztmarketapi-0.2.1/lztmarketapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 04:05:58.621119 lztmarketapi-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-06-13 04:05:46.000000 lztmarketapi-0.2.1/setup.py
```

### Comparing `lztmarketapi-0.2.0/LICENSE.txt` & `lztmarketapi-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/PKG-INFO` & `lztmarketapi-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lztmarketapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Данная библиотека создана для взаимодействия с api lzt.market.
 Home-page: https://github.com/KazariFox/AsyncMarketLztApi
 Author: KazariFox
 Author-email: 
 License: apache-2.0
 Keywords: lzt,lolzteam,lolzteam market,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lztmarketapi-0.2.0/README.md` & `lztmarketapi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/ApiWrapper/__init__.py` & `lztmarketapi-0.2.1/lztmarketapi/ApiWrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/BaseGame.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/BaseGame.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Battlenet.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/VPN.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
-class Battlenet(BaseGame):
+class VPN(BaseGame):
 
     def __init__(self, wrapper) -> None:
         super().__init__(wrapper)
-        self.categ_obj = Category.BATTLENET
+        self.categ_obj = Category.VPN
         self.name = self.categ_obj.name
         self.categ_id = self.categ_obj.id
 
     async def search(self, page: int = 1, pmin: int | None = None, pmax: int | None = None, title: str | None = None, parse_sticky_items: bool | None = None, parse_same_items: bool | None = None, game: list[int] | None = None, **kwargs) -> List[AccountManager]:
         """game (array) - List of games
 
 daybreak (number) - Number of days the account has been offline
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Blitz.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Blitz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Blitz(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Cinema.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/YouTube.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
-class Cinema(BaseGame):
+class YouTube(BaseGame):
 
     def __init__(self, wrapper) -> None:
         super().__init__(wrapper)
-        self.categ_obj = Category.ONLINE_CINEMA
+        self.categ_obj = Category.YOUTUBE
         self.name = self.categ_obj.name
         self.categ_id = self.categ_obj.id
 
     async def search(self, page: int = 1, pmin: int | None = None, pmax: int | None = None, title: str | None = None, parse_sticky_items: bool | None = None, parse_same_items: bool | None = None, game: list[int] | None = None, **kwargs) -> List[AccountManager]:
         return await super().search(page, pmin, pmax, title, parse_sticky_items, parse_same_items, game, **kwargs)
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Discord.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Discord.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Discord(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/EpicGames.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Telegram.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
-class EpicGames(BaseGame):
+class Telegram(BaseGame):
 
     def __init__(self, wrapper) -> None:
         super().__init__(wrapper)
-        self.categ_obj = Category.EPIC_GAMES
-        
+        self.categ_obj = Category.TELEGRAM
         self.name = self.categ_obj.name
         self.categ_id = self.categ_obj.id
 
     async def search(self, page: int = 1, pmin: int | None = None, pmax: int | None = None, title: str | None = None, parse_sticky_items: bool | None = None, parse_same_items: bool | None = None, game: list[int] | None = None, **kwargs) -> List[AccountManager]:
-        """game (array) - List of games
+        """scam (boolean) - Has a scam badge
+
+spam (boolean) - Has a spam ban
+
+password (boolean) - Has a cloud password
+
+premium (boolean) - Has a premium subscription
+
+country[] (array) - List of allowed countries
 
-change_email (boolean) - You can change email
+not_country[] (array) - List of disallowed countries
 
-rl_purchases (boolean) - Has Rocket League purchases"""
+daybreak (number) - Number of days the account has been offline"""
         return await super().search(page, pmin, pmax, title, parse_sticky_items, parse_same_items, game, **kwargs)
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class EscapeFromTarkov(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Fortnite.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Fortnite.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Fortnite(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class GenshinImpact(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Instagram.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Instagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Instagram(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Origin.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Origin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Origin(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/SocialClub.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/SocialClub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class SocialClub(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Spotify.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Spotify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Spotify(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Steam.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Steam.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Supercell.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Supercell.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Supercell(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Telegram.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Uplay.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
-class Telegram(BaseGame):
+class Uplay(BaseGame):
 
     def __init__(self, wrapper) -> None:
         super().__init__(wrapper)
-        self.categ_obj = Category.TELEGRAM
+        self.categ_obj = Category.UPLAY
         self.name = self.categ_obj.name
         self.categ_id = self.categ_obj.id
 
     async def search(self, page: int = 1, pmin: int | None = None, pmax: int | None = None, title: str | None = None, parse_sticky_items: bool | None = None, parse_same_items: bool | None = None, game: list[int] | None = None, **kwargs) -> List[AccountManager]:
-        """scam (boolean) - Has a scam badge
-
-spam (boolean) - Has a spam ban
-
-password (boolean) - Has a cloud password
-
-premium (boolean) - Has a premium subscription
+        """game[] (array) - List of games
 
 country[] (array) - List of allowed countries
 
 not_country[] (array) - List of disallowed countries
 
-daybreak (number) - Number of days the account has been offline"""
+daybreak (number) - Number of days the account has been offline
+
+r6_level_min (number) - Minimum level in Tom Clancy's Rainbow Six Siege
+
+r6_level_max (number) - Maximum level in Tom Clancy's Rainbow Six Siege"""
         return await super().search(page, pmin, pmax, title, parse_sticky_items, parse_same_items, game, **kwargs)
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/TikTok.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/TikTok.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class TikTok(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Uplay.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/EpicGames.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
-class Uplay(BaseGame):
+class EpicGames(BaseGame):
 
     def __init__(self, wrapper) -> None:
         super().__init__(wrapper)
-        self.categ_obj = Category.UPLAY
+        self.categ_obj = Category.EPIC_GAMES
+        
         self.name = self.categ_obj.name
         self.categ_id = self.categ_obj.id
 
     async def search(self, page: int = 1, pmin: int | None = None, pmax: int | None = None, title: str | None = None, parse_sticky_items: bool | None = None, parse_same_items: bool | None = None, game: list[int] | None = None, **kwargs) -> List[AccountManager]:
-        """game[] (array) - List of games
-
-country[] (array) - List of allowed countries
-
-not_country[] (array) - List of disallowed countries
-
-daybreak (number) - Number of days the account has been offline
+        """game (array) - List of games
 
-r6_level_min (number) - Minimum level in Tom Clancy's Rainbow Six Siege
+change_email (boolean) - You can change email
 
-r6_level_max (number) - Maximum level in Tom Clancy's Rainbow Six Siege"""
+rl_purchases (boolean) - Has Rocket League purchases"""
         return await super().search(page, pmin, pmax, title, parse_sticky_items, parse_same_items, game, **kwargs)
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/VK.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/VK.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import List
 
-from lztmarket.Types import Good
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class VK(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/VPN.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Battlenet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
-class VPN(BaseGame):
+class Battlenet(BaseGame):
 
     def __init__(self, wrapper) -> None:
         super().__init__(wrapper)
-        self.categ_obj = Category.VPN
+        self.categ_obj = Category.BATTLENET
         self.name = self.categ_obj.name
         self.categ_id = self.categ_obj.id
 
     async def search(self, page: int = 1, pmin: int | None = None, pmax: int | None = None, title: str | None = None, parse_sticky_items: bool | None = None, parse_same_items: bool | None = None, game: list[int] | None = None, **kwargs) -> List[AccountManager]:
         """game (array) - List of games
 
 daybreak (number) - Number of days the account has been offline
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Valorant.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Valorant.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Valorant(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/WarThunder.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/WarThunder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class WarThunder(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Warface.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Warface.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class Warface(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
 class WorldOfTanks(BaseGame):
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/YouTube.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/Cinema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List
 
-from lztmarket.Types import Good
+
 from ....Types import Good, Category
 from .BaseGame import BaseGame
 from ....Types.AccountManage import AccountManager
 
 
-class YouTube(BaseGame):
+class Cinema(BaseGame):
 
     def __init__(self, wrapper) -> None:
         super().__init__(wrapper)
-        self.categ_obj = Category.YOUTUBE
+        self.categ_obj = Category.ONLINE_CINEMA
         self.name = self.categ_obj.name
         self.categ_id = self.categ_obj.id
 
     async def search(self, page: int = 1, pmin: int | None = None, pmax: int | None = None, title: str | None = None, parse_sticky_items: bool | None = None, parse_same_items: bool | None = None, game: list[int] | None = None, **kwargs) -> List[AccountManager]:
         return await super().search(page, pmin, pmax, title, parse_sticky_items, parse_same_items, game, **kwargs)
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/__init__.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/GamesModels/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Games/__init__.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Games/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Good/__init__.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Good/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Client/Payment/__init__.py` & `lztmarketapi-0.2.1/lztmarketapi/Client/Payment/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Types/AccountManage/__init__.py` & `lztmarketapi-0.2.1/lztmarketapi/Types/AccountManage/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Types/Category.py` & `lztmarketapi-0.2.1/lztmarketapi/Types/Category.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Types/Good.py` & `lztmarketapi-0.2.1/lztmarketapi/Types/Good.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Types/PaymentModel/__init__.py` & `lztmarketapi-0.2.1/lztmarketapi/Types/PaymentModel/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Types/Profile.py` & `lztmarketapi-0.2.1/lztmarketapi/Types/Profile.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi/Utils/Response.py` & `lztmarketapi-0.2.1/lztmarketapi/Utils/Response.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/lztmarketapi.egg-info/PKG-INFO` & `lztmarketapi-0.2.1/lztmarketapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lztmarketapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Данная библиотека создана для взаимодействия с api lzt.market.
 Home-page: https://github.com/KazariFox/AsyncMarketLztApi
 Author: KazariFox
 Author-email: 
 License: apache-2.0
 Keywords: lzt,lolzteam,lolzteam market,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lztmarketapi-0.2.0/lztmarketapi.egg-info/SOURCES.txt` & `lztmarketapi-0.2.1/lztmarketapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.0/setup.py` & `lztmarketapi-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # from distutils.core import setup
 from setuptools import setup, find_packages
 setup(
   name = 'lztmarketapi',        
   packages = find_packages(),
   include_package_data=True,
-  version = '0.2.0',    
+  version = '0.2.1',    
   license='apache-2.0',      
   description = 'Данная библиотека создана для взаимодействия с api lzt.market.',   
   author = 'KazariFox',                  
   author_email = '',     
   url = 'https://github.com/KazariFox/AsyncMarketLztApi',   
   keywords = ['lzt', 'lolzteam', 'lolzteam market', 'api'],  
   install_requires=[
```

