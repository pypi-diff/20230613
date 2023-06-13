# Comparing `tmp/lztmarketapi-0.2.2.tar.gz` & `tmp/lztmarketapi-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lztmarketapi-0.2.2.tar", last modified: Tue Jun 13 05:02:14 2023, max compression
+gzip compressed data, was "lztmarketapi-0.2.2.1.tar", last modified: Tue Jun 13 05:05:12 2023, max compression
```

## Comparing `lztmarketapi-0.2.2.tar` & `lztmarketapi-0.2.2.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:14.017917 lztmarketapi-0.2.2/
--rw-rw-rw-   0        0        0    11558 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      611 2023-06-13 05:02:14.017917 lztmarketapi-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     5603 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.955809 lztmarketapi-0.2.2/lztmarketapi/
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.962826 lztmarketapi-0.2.2/lztmarketapi/ApiWrapper/
--rw-rw-rw-   0        0        0       86 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/ApiWrapper/ApiExceptions.py
--rw-rw-rw-   0        0        0     3690 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/ApiWrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.962826 lztmarketapi-0.2.2/lztmarketapi/Client/
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.963824 lztmarketapi-0.2.2/lztmarketapi/Client/Games/
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.992802 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/
--rw-rw-rw-   0        0        0     2101 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/BaseGame.py
--rw-rw-rw-   0        0        0     1421 2023-06-13 04:05:15.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Battlenet.py
--rw-rw-rw-   0        0        0     1715 2023-06-13 04:05:14.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Blitz.py
--rw-rw-rw-   0        0        0      771 2023-06-13 04:05:13.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Cinema.py
--rw-rw-rw-   0        0        0     1442 2023-06-13 04:05:13.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Discord.py
--rw-rw-rw-   0        0        0      930 2023-06-13 04:05:13.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/EpicGames.py
--rw-rw-rw-   0        0        0     1071 2023-06-13 04:05:12.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py
--rw-rw-rw-   0        0        0     1803 2023-06-13 04:05:12.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Fortnite.py
--rw-rw-rw-   0        0        0     1682 2023-06-13 04:05:12.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py
--rw-rw-rw-   0        0        0     1311 2023-06-13 04:05:11.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Instagram.py
--rw-rw-rw-   0        0        0     1318 2023-06-13 04:05:11.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Origin.py
--rw-rw-rw-   0        0        0      928 2023-06-13 04:05:10.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/SocialClub.py
--rw-rw-rw-   0        0        0     1397 2023-06-13 04:05:10.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Spotify.py
--rw-rw-rw-   0        0        0     4850 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Steam.py
--rw-rw-rw-   0        0        0     1121 2023-06-13 04:05:09.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Supercell.py
--rw-rw-rw-   0        0        0     1119 2023-06-13 04:05:09.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Telegram.py
--rw-rw-rw-   0        0        0     1449 2023-06-13 04:05:09.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/TikTok.py
--rw-rw-rw-   0        0        0     1130 2023-06-13 04:05:08.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Uplay.py
--rw-rw-rw-   0        0        0     2239 2023-06-13 04:03:55.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/VK.py
--rw-rw-rw-   0        0        0     1409 2023-06-13 04:05:06.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/VPN.py
--rw-rw-rw-   0        0        0     1868 2023-06-13 04:05:08.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Valorant.py
--rw-rw-rw-   0        0        0     1572 2023-06-13 04:05:05.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/WarThunder.py
--rw-rw-rw-   0        0        0     1050 2023-06-13 04:05:06.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Warface.py
--rw-rw-rw-   0        0        0     1716 2023-06-13 04:05:06.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py
--rw-rw-rw-   0        0        0      766 2023-06-13 04:05:05.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/YouTube.py
--rw-rw-rw-   0        0        0      760 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/__init__.py
--rw-rw-rw-   0        0        0     1901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.993810 lztmarketapi-0.2.2/lztmarketapi/Client/Good/
--rw-rw-rw-   0        0        0     2689 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Good/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.994809 lztmarketapi-0.2.2/lztmarketapi/Client/Me/
--rw-rw-rw-   0        0        0      369 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Me/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.995797 lztmarketapi-0.2.2/lztmarketapi/Client/Payment/
--rw-rw-rw-   0        0        0     6973 2023-06-13 05:00:03.000000 lztmarketapi-0.2.2/lztmarketapi/Client/Payment/__init__.py
--rw-rw-rw-   0        0        0      495 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:14.012919 lztmarketapi-0.2.2/lztmarketapi/Types/
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:14.014918 lztmarketapi-0.2.2/lztmarketapi/Types/AccountManage/
--rw-rw-rw-   0        0        0      134 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/AccountManage/ManageExceptions.py
--rw-rw-rw-   0        0        0    15293 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/AccountManage/__init__.py
--rw-rw-rw-   0        0        0     1229 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/Category.py
--rw-rw-rw-   0        0        0      106 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/Currency.py
--rw-rw-rw-   0        0        0     6474 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/Good.py
--rw-rw-rw-   0        0        0       36 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/Guarantee.py
--rw-rw-rw-   0        0        0      141 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/ItemOrigin.py
--rw-rw-rw-   0        0        0       38 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/Mail.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:14.015918 lztmarketapi-0.2.2/lztmarketapi/Types/PaymentModel/
--rw-rw-rw-   0        0        0      901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/PaymentModel/__init__.py
--rw-rw-rw-   0        0        0      279 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/PaymentType.py
--rw-rw-rw-   0        0        0      724 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/Profile.py
--rw-rw-rw-   0        0        0       21 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/Result.py
--rw-rw-rw-   0        0        0       75 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/TimeValues.py
--rw-rw-rw-   0        0        0      349 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Types/User.py
--rw-rw-rw-   0        0        0       15 2023-06-13 03:58:47.000000 lztmarketapi-0.2.2/lztmarketapi/Types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:14.016917 lztmarketapi-0.2.2/lztmarketapi/Utils/
--rw-rw-rw-   0        0        0      906 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2/lztmarketapi/Utils/Response.py
--rw-rw-rw-   0        0        0       15 2023-06-13 03:59:13.000000 lztmarketapi-0.2.2/lztmarketapi/Utils/__init__.py
--rw-rw-rw-   0        0        0      299 2023-06-13 03:57:53.000000 lztmarketapi-0.2.2/lztmarketapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:02:13.960820 lztmarketapi-0.2.2/lztmarketapi.egg-info/
--rw-rw-rw-   0        0        0      611 2023-06-13 05:02:13.000000 lztmarketapi-0.2.2/lztmarketapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2367 2023-06-13 05:02:13.000000 lztmarketapi-0.2.2/lztmarketapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 05:02:13.000000 lztmarketapi-0.2.2/lztmarketapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 05:02:13.000000 lztmarketapi-0.2.2/lztmarketapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 05:02:13.000000 lztmarketapi-0.2.2/lztmarketapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 05:02:14.017917 lztmarketapi-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-06-13 05:02:11.000000 lztmarketapi-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.218254 lztmarketapi-0.2.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      613 2023-06-13 05:05:12.218254 lztmarketapi-0.2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5603 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.170245 lztmarketapi-0.2.2.1/lztmarketapi/
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.170245 lztmarketapi-0.2.2.1/lztmarketapi/ApiWrapper/
+-rw-rw-rw-   0        0        0       86 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/ApiWrapper/ApiExceptions.py
+-rw-rw-rw-   0        0        0     3690 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/ApiWrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.170245 lztmarketapi-0.2.2.1/lztmarketapi/Client/
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.178236 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.194250 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/
+-rw-rw-rw-   0        0        0     2101 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/BaseGame.py
+-rw-rw-rw-   0        0        0     1421 2023-06-13 04:05:15.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Battlenet.py
+-rw-rw-rw-   0        0        0     1715 2023-06-13 04:05:14.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Blitz.py
+-rw-rw-rw-   0        0        0      771 2023-06-13 04:05:13.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Cinema.py
+-rw-rw-rw-   0        0        0     1442 2023-06-13 04:05:13.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Discord.py
+-rw-rw-rw-   0        0        0      930 2023-06-13 04:05:13.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/EpicGames.py
+-rw-rw-rw-   0        0        0     1071 2023-06-13 04:05:12.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py
+-rw-rw-rw-   0        0        0     1803 2023-06-13 04:05:12.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Fortnite.py
+-rw-rw-rw-   0        0        0     1682 2023-06-13 04:05:12.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py
+-rw-rw-rw-   0        0        0     1311 2023-06-13 04:05:11.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Instagram.py
+-rw-rw-rw-   0        0        0     1318 2023-06-13 04:05:11.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Origin.py
+-rw-rw-rw-   0        0        0      928 2023-06-13 04:05:10.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/SocialClub.py
+-rw-rw-rw-   0        0        0     1397 2023-06-13 04:05:10.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Spotify.py
+-rw-rw-rw-   0        0        0     4850 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Steam.py
+-rw-rw-rw-   0        0        0     1121 2023-06-13 04:05:09.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Supercell.py
+-rw-rw-rw-   0        0        0     1119 2023-06-13 04:05:09.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Telegram.py
+-rw-rw-rw-   0        0        0     1449 2023-06-13 04:05:09.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/TikTok.py
+-rw-rw-rw-   0        0        0     1130 2023-06-13 04:05:08.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Uplay.py
+-rw-rw-rw-   0        0        0     2239 2023-06-13 04:03:55.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/VK.py
+-rw-rw-rw-   0        0        0     1409 2023-06-13 04:05:06.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/VPN.py
+-rw-rw-rw-   0        0        0     1868 2023-06-13 04:05:08.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Valorant.py
+-rw-rw-rw-   0        0        0     1572 2023-06-13 04:05:05.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/WarThunder.py
+-rw-rw-rw-   0        0        0     1050 2023-06-13 04:05:06.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Warface.py
+-rw-rw-rw-   0        0        0     1716 2023-06-13 04:05:06.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py
+-rw-rw-rw-   0        0        0      766 2023-06-13 04:05:05.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/YouTube.py
+-rw-rw-rw-   0        0        0      760 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/__init__.py
+-rw-rw-rw-   0        0        0     1901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.202255 lztmarketapi-0.2.2.1/lztmarketapi/Client/Good/
+-rw-rw-rw-   0        0        0     2689 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Good/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.202255 lztmarketapi-0.2.2.1/lztmarketapi/Client/Me/
+-rw-rw-rw-   0        0        0      369 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Me/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.202255 lztmarketapi-0.2.2.1/lztmarketapi/Client/Payment/
+-rw-rw-rw-   0        0        0     6972 2023-06-13 05:04:43.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/Payment/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.210250 lztmarketapi-0.2.2.1/lztmarketapi/Types/
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.210250 lztmarketapi-0.2.2.1/lztmarketapi/Types/AccountManage/
+-rw-rw-rw-   0        0        0      134 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/AccountManage/ManageExceptions.py
+-rw-rw-rw-   0        0        0    15293 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/AccountManage/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/Category.py
+-rw-rw-rw-   0        0        0      106 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/Currency.py
+-rw-rw-rw-   0        0        0     6474 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/Good.py
+-rw-rw-rw-   0        0        0       36 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/Guarantee.py
+-rw-rw-rw-   0        0        0      141 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/ItemOrigin.py
+-rw-rw-rw-   0        0        0       38 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/Mail.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.210250 lztmarketapi-0.2.2.1/lztmarketapi/Types/PaymentModel/
+-rw-rw-rw-   0        0        0      901 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/PaymentModel/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/PaymentType.py
+-rw-rw-rw-   0        0        0      724 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/Profile.py
+-rw-rw-rw-   0        0        0       21 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/Result.py
+-rw-rw-rw-   0        0        0       75 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/TimeValues.py
+-rw-rw-rw-   0        0        0      349 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/User.py
+-rw-rw-rw-   0        0        0       15 2023-06-13 03:58:47.000000 lztmarketapi-0.2.2.1/lztmarketapi/Types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.218254 lztmarketapi-0.2.2.1/lztmarketapi/Utils/
+-rw-rw-rw-   0        0        0      906 2023-06-13 03:32:21.000000 lztmarketapi-0.2.2.1/lztmarketapi/Utils/Response.py
+-rw-rw-rw-   0        0        0       15 2023-06-13 03:59:13.000000 lztmarketapi-0.2.2.1/lztmarketapi/Utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-06-13 03:57:53.000000 lztmarketapi-0.2.2.1/lztmarketapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:05:12.170245 lztmarketapi-0.2.2.1/lztmarketapi.egg-info/
+-rw-rw-rw-   0        0        0      613 2023-06-13 05:05:12.000000 lztmarketapi-0.2.2.1/lztmarketapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2367 2023-06-13 05:05:12.000000 lztmarketapi-0.2.2.1/lztmarketapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 05:05:12.000000 lztmarketapi-0.2.2.1/lztmarketapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 05:05:12.000000 lztmarketapi-0.2.2.1/lztmarketapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 05:05:12.000000 lztmarketapi-0.2.2.1/lztmarketapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 05:05:12.218254 lztmarketapi-0.2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      914 2023-06-13 05:05:00.000000 lztmarketapi-0.2.2.1/setup.py
```

### Comparing `lztmarketapi-0.2.2/LICENSE.txt` & `lztmarketapi-0.2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/PKG-INFO` & `lztmarketapi-0.2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lztmarketapi
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Данная библиотека создана для взаимодействия с api lzt.market.
 Home-page: https://github.com/KazariFox/AsyncMarketLztApi
 Author: KazariFox
 Author-email: 
 License: apache-2.0
 Keywords: lzt,lolzteam,lolzteam market,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lztmarketapi-0.2.2/README.md` & `lztmarketapi-0.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/ApiWrapper/__init__.py` & `lztmarketapi-0.2.2.1/lztmarketapi/ApiWrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/BaseGame.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/BaseGame.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Battlenet.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Battlenet.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Blitz.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Blitz.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Cinema.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Cinema.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Discord.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Discord.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/EpicGames.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/EpicGames.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/EscapeFromTarkov.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Fortnite.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Fortnite.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/GenshinImpact.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Instagram.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Instagram.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Origin.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Origin.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/SocialClub.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/SocialClub.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Spotify.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Spotify.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Steam.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Steam.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Supercell.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Supercell.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Telegram.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Telegram.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/TikTok.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/TikTok.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Uplay.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Uplay.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/VK.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/VK.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/VPN.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/VPN.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Valorant.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Valorant.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/WarThunder.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/WarThunder.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/Warface.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/Warface.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/WorldOfTanks.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/YouTube.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/YouTube.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/GamesModels/__init__.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/GamesModels/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Games/__init__.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Games/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Good/__init__.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Good/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Client/Payment/__init__.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Client/Payment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         if endDate:
             params['endDate'] = endDate
 
         if wallet:
             params['wallet'] = wallet
 
         if comment:
-            comment['comment'] = comment
+            params['comment'] = comment
 
         if is_hold is not None:
             params['is_hold'] = int(is_hold)
 
         if start_by_operation_id:
             params['operation_id_lt'] = start_by_operation_id
```

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Types/AccountManage/__init__.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Types/AccountManage/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Types/Category.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Types/Category.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Types/Good.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Types/Good.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Types/PaymentModel/__init__.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Types/PaymentModel/__init__.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Types/Profile.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Types/Profile.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi/Utils/Response.py` & `lztmarketapi-0.2.2.1/lztmarketapi/Utils/Response.py`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/lztmarketapi.egg-info/PKG-INFO` & `lztmarketapi-0.2.2.1/lztmarketapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lztmarketapi
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Данная библиотека создана для взаимодействия с api lzt.market.
 Home-page: https://github.com/KazariFox/AsyncMarketLztApi
 Author: KazariFox
 Author-email: 
 License: apache-2.0
 Keywords: lzt,lolzteam,lolzteam market,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lztmarketapi-0.2.2/lztmarketapi.egg-info/SOURCES.txt` & `lztmarketapi-0.2.2.1/lztmarketapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lztmarketapi-0.2.2/setup.py` & `lztmarketapi-0.2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # from distutils.core import setup
 from setuptools import setup, find_packages
 setup(
   name = 'lztmarketapi',        
   packages = find_packages(),
   include_package_data=True,
-  version = '0.2.2',    
+  version = '0.2.2.1',    
   license='apache-2.0',      
   description = 'Данная библиотека создана для взаимодействия с api lzt.market.',   
   author = 'KazariFox',                  
   author_email = '',     
   url = 'https://github.com/KazariFox/AsyncMarketLztApi',   
   keywords = ['lzt', 'lolzteam', 'lolzteam market', 'api'],  
   install_requires=[
```

