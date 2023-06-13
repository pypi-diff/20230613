# Comparing `tmp/lztmarketapi-0.1b0.tar.gz` & `tmp/lztmarketapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lztmarketapi-0.1b0.tar", last modified: Tue Jun 13 03:53:59 2023, max compression
+gzip compressed data, was "lztmarketapi-0.2.0.tar", last modified: Tue Jun 13 03:59:42 2023, max compression
```

## Comparing `lztmarketapi-0.1b0.tar` & `lztmarketapi-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.338796 lztmarketapi-0.1b0/
--rw-rw-rw-   0        0        0    11558 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/LICENSE.txt
--rw-rw-rw-   0        0        0      611 2023-06-13 03:53:59.338796 lztmarketapi-0.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     5603 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.279815 lztmarketapi-0.1b0/lztmarketapi/
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.292810 lztmarketapi-0.1b0/lztmarketapi/ApiWrapper/
--rw-rw-rw-   0        0        0       86 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/ApiWrapper/ApiExceptions.py
--rw-rw-rw-   0        0        0     3690 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/ApiWrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.294811 lztmarketapi-0.1b0/lztmarketapi/Client/
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.295811 lztmarketapi-0.1b0/lztmarketapi/Client/Games/
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.332798 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/
--rw-rw-rw-   0        0        0     2101 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/BaseGame.py
--rw-rw-rw-   0        0        0     1453 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Battlenet.py
--rw-rw-rw-   0        0        0     1747 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Blitz.py
--rw-rw-rw-   0        0        0      803 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Cinema.py
--rw-rw-rw-   0        0        0     1474 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Discord.py
--rw-rw-rw-   0        0        0      962 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/EpicGames.py
--rw-rw-rw-   0        0        0     1103 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py
--rw-rw-rw-   0        0        0     1835 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Fortnite.py
--rw-rw-rw-   0        0        0     1714 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py
--rw-rw-rw-   0        0        0     1343 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Instagram.py
--rw-rw-rw-   0        0        0     1350 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Origin.py
--rw-rw-rw-   0        0        0      960 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/SocialClub.py
--rw-rw-rw-   0        0        0     1429 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Spotify.py
--rw-rw-rw-   0        0        0     4850 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Steam.py
--rw-rw-rw-   0        0        0     1153 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Supercell.py
--rw-rw-rw-   0        0        0     1151 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Telegram.py
--rw-rw-rw-   0        0        0     1481 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/TikTok.py
--rw-rw-rw-   0        0        0     1162 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Uplay.py
--rw-rw-rw-   0        0        0     2273 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/VK.py
--rw-rw-rw-   0        0        0     1441 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/VPN.py
--rw-rw-rw-   0        0        0     1898 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Valorant.py
--rw-rw-rw-   0        0        0     1604 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/WarThunder.py
--rw-rw-rw-   0        0        0     1082 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Warface.py
--rw-rw-rw-   0        0        0     1748 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py
--rw-rw-rw-   0        0        0      798 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/YouTube.py
--rw-rw-rw-   0        0        0      760 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/__init__.py
--rw-rw-rw-   0        0        0     1901 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.334797 lztmarketapi-0.1b0/lztmarketapi/Client/Good/
--rw-rw-rw-   0        0        0     2689 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Good/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.336797 lztmarketapi-0.1b0/lztmarketapi/Client/Me/
--rw-rw-rw-   0        0        0      369 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Me/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.337796 lztmarketapi-0.1b0/lztmarketapi/Client/Payment/
--rw-rw-rw-   0        0        0     7001 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/Payment/__init__.py
--rw-rw-rw-   0        0        0      495 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/Client/__init__.py
--rw-rw-rw-   0        0        0      237 2023-06-13 03:32:21.000000 lztmarketapi-0.1b0/lztmarketapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:53:59.290811 lztmarketapi-0.1b0/lztmarketapi.egg-info/
--rw-rw-rw-   0        0        0      611 2023-06-13 03:53:59.000000 lztmarketapi-0.1b0/lztmarketapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2023-06-13 03:53:59.000000 lztmarketapi-0.1b0/lztmarketapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 03:53:59.000000 lztmarketapi-0.1b0/lztmarketapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 03:53:59.000000 lztmarketapi-0.1b0/lztmarketapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 03:53:59.000000 lztmarketapi-0.1b0/lztmarketapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 03:53:59.339795 lztmarketapi-0.1b0/setup.cfg
--rw-rw-rw-   0        0        0      911 2023-06-13 03:53:56.000000 lztmarketapi-0.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.236247 lztmarketapi-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      611 2023-06-13 03:59:42.236247 lztmarketapi-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5603 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.142279 lztmarketapi-0.2.0/lztmarketapi/
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.152275 lztmarketapi-0.2.0/lztmarketapi/ApiWrapper/
+-rw-rw-rw-   0        0        0       86 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/ApiWrapper/ApiExceptions.py
+-rw-rw-rw-   0        0        0     3690 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/ApiWrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.154274 lztmarketapi-0.2.0/lztmarketapi/Client/
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.155274 lztmarketapi-0.2.0/lztmarketapi/Client/Games/
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.205257 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/
+-rw-rw-rw-   0        0        0     2101 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/BaseGame.py
+-rw-rw-rw-   0        0        0     1453 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Battlenet.py
+-rw-rw-rw-   0        0        0     1747 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Blitz.py
+-rw-rw-rw-   0        0        0      803 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Cinema.py
+-rw-rw-rw-   0        0        0     1474 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Discord.py
+-rw-rw-rw-   0        0        0      962 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/EpicGames.py
+-rw-rw-rw-   0        0        0     1103 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py
+-rw-rw-rw-   0        0        0     1835 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Fortnite.py
+-rw-rw-rw-   0        0        0     1714 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py
+-rw-rw-rw-   0        0        0     1343 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Instagram.py
+-rw-rw-rw-   0        0        0     1350 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Origin.py
+-rw-rw-rw-   0        0        0      960 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/SocialClub.py
+-rw-rw-rw-   0        0        0     1429 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Spotify.py
+-rw-rw-rw-   0        0        0     4850 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Steam.py
+-rw-rw-rw-   0        0        0     1153 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Supercell.py
+-rw-rw-rw-   0        0        0     1151 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Telegram.py
+-rw-rw-rw-   0        0        0     1481 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/TikTok.py
+-rw-rw-rw-   0        0        0     1162 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Uplay.py
+-rw-rw-rw-   0        0        0     2273 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/VK.py
+-rw-rw-rw-   0        0        0     1441 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/VPN.py
+-rw-rw-rw-   0        0        0     1898 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Valorant.py
+-rw-rw-rw-   0        0        0     1604 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/WarThunder.py
+-rw-rw-rw-   0        0        0     1082 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Warface.py
+-rw-rw-rw-   0        0        0     1748 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py
+-rw-rw-rw-   0        0        0      798 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/YouTube.py
+-rw-rw-rw-   0        0        0      760 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/__init__.py
+-rw-rw-rw-   0        0        0     1901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.206258 lztmarketapi-0.2.0/lztmarketapi/Client/Good/
+-rw-rw-rw-   0        0        0     2689 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Good/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.207257 lztmarketapi-0.2.0/lztmarketapi/Client/Me/
+-rw-rw-rw-   0        0        0      369 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Me/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.208257 lztmarketapi-0.2.0/lztmarketapi/Client/Payment/
+-rw-rw-rw-   0        0        0     7001 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/Payment/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.230250 lztmarketapi-0.2.0/lztmarketapi/Types/
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.232248 lztmarketapi-0.2.0/lztmarketapi/Types/AccountManage/
+-rw-rw-rw-   0        0        0      134 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/AccountManage/ManageExceptions.py
+-rw-rw-rw-   0        0        0    15293 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/AccountManage/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Category.py
+-rw-rw-rw-   0        0        0      106 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Currency.py
+-rw-rw-rw-   0        0        0     6474 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Good.py
+-rw-rw-rw-   0        0        0       36 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Guarantee.py
+-rw-rw-rw-   0        0        0      141 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/ItemOrigin.py
+-rw-rw-rw-   0        0        0       38 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Mail.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.233250 lztmarketapi-0.2.0/lztmarketapi/Types/PaymentModel/
+-rw-rw-rw-   0        0        0      901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/PaymentModel/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/PaymentType.py
+-rw-rw-rw-   0        0        0      724 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Profile.py
+-rw-rw-rw-   0        0        0       21 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/Result.py
+-rw-rw-rw-   0        0        0       75 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/TimeValues.py
+-rw-rw-rw-   0        0        0      349 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Types/User.py
+-rw-rw-rw-   0        0        0       15 2023-06-13 03:58:47.000000 lztmarketapi-0.2.0/lztmarketapi/Types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.235248 lztmarketapi-0.2.0/lztmarketapi/Utils/
+-rw-rw-rw-   0        0        0      906 2023-06-13 03:32:21.000000 lztmarketapi-0.2.0/lztmarketapi/Utils/Response.py
+-rw-rw-rw-   0        0        0       15 2023-06-13 03:59:13.000000 lztmarketapi-0.2.0/lztmarketapi/Utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-06-13 03:57:53.000000 lztmarketapi-0.2.0/lztmarketapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:59:42.149276 lztmarketapi-0.2.0/lztmarketapi.egg-info/
+-rw-rw-rw-   0        0        0      611 2023-06-13 03:59:41.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2367 2023-06-13 03:59:42.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 03:59:41.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 03:59:41.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 03:59:41.000000 lztmarketapi-0.2.0/lztmarketapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 03:59:42.237247 lztmarketapi-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-06-13 03:56:29.000000 lztmarketapi-0.2.0/setup.py
```

### Comparing `lztmarketapi-0.1b0/LICENSE.txt` & `lztmarketapi-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/PKG-INFO` & `lztmarketapi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lztmarketapi
-Version: 0.1b0
+Version: 0.2.0
 Summary: Данная библиотека создана для взаимодействия с api lzt.market.
 Home-page: https://github.com/KazariFox/AsyncMarketLztApi
 Author: KazariFox
 Author-email: 
 License: apache-2.0
 Keywords: lzt,lolzteam,lolzteam market,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lztmarketapi-0.1b0/README.md` & `lztmarketapi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/ApiWrapper/__init__.py` & `lztmarketapi-0.2.0/lztmarketapi/ApiWrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/BaseGame.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/BaseGame.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Battlenet.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Battlenet.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Blitz.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Blitz.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Cinema.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Cinema.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Discord.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Discord.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/EpicGames.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/EpicGames.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Fortnite.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Fortnite.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Instagram.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Instagram.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Origin.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Origin.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/SocialClub.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/SocialClub.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Spotify.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Spotify.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Steam.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Steam.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Supercell.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Supercell.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Telegram.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Telegram.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/TikTok.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/TikTok.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Uplay.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Uplay.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/VK.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/VK.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/VPN.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/VPN.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Valorant.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Valorant.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/WarThunder.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/WarThunder.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/Warface.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/Warface.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/YouTube.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/YouTube.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/GamesModels/__init__.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/GamesModels/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Games/__init__.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Games/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Good/__init__.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Good/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi/Client/Payment/__init__.py` & `lztmarketapi-0.2.0/lztmarketapi/Client/Payment/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.1b0/lztmarketapi.egg-info/PKG-INFO` & `lztmarketapi-0.2.0/lztmarketapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lztmarketapi
-Version: 0.1b0
+Version: 0.2.0
 Summary: Данная библиотека создана для взаимодействия с api lzt.market.
 Home-page: https://github.com/KazariFox/AsyncMarketLztApi
 Author: KazariFox
 Author-email: 
 License: apache-2.0
 Keywords: lzt,lolzteam,lolzteam market,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lztmarketapi-0.1b0/lztmarketapi.egg-info/SOURCES.txt` & `lztmarketapi-0.2.0/lztmarketapi.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -36,8 +36,25 @@
 lztmarketapi/Client/Games/GamesModels/WarThunder.py
 lztmarketapi/Client/Games/GamesModels/Warface.py
 lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py
 lztmarketapi/Client/Games/GamesModels/YouTube.py
 lztmarketapi/Client/Games/GamesModels/__init__.py
 lztmarketapi/Client/Good/__init__.py
 lztmarketapi/Client/Me/__init__.py
-lztmarketapi/Client/Payment/__init__.py
+lztmarketapi/Client/Payment/__init__.py
+lztmarketapi/Types/Category.py
+lztmarketapi/Types/Currency.py
+lztmarketapi/Types/Good.py
+lztmarketapi/Types/Guarantee.py
+lztmarketapi/Types/ItemOrigin.py
+lztmarketapi/Types/Mail.py
+lztmarketapi/Types/PaymentType.py
+lztmarketapi/Types/Profile.py
+lztmarketapi/Types/Result.py
+lztmarketapi/Types/TimeValues.py
+lztmarketapi/Types/User.py
+lztmarketapi/Types/__init__.py
+lztmarketapi/Types/AccountManage/ManageExceptions.py
+lztmarketapi/Types/AccountManage/__init__.py
+lztmarketapi/Types/PaymentModel/__init__.py
+lztmarketapi/Utils/Response.py
+lztmarketapi/Utils/__init__.py
```

### Comparing `lztmarketapi-0.1b0/setup.py` & `lztmarketapi-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # from distutils.core import setup
 from setuptools import setup, find_packages
 setup(
   name = 'lztmarketapi',        
   packages = find_packages(),
   include_package_data=True,
-  version = '0.1b',    
+  version = '0.2.0',    
   license='apache-2.0',      
   description = 'Данная библиотека создана для взаимодействия с api lzt.market.',   
   author = 'KazariFox',                  
   author_email = '',     
   url = 'https://github.com/KazariFox/AsyncMarketLztApi',   
   keywords = ['lzt', 'lolzteam', 'lolzteam market', 'api'],  
   install_requires=[
```

