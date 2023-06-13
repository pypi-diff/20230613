# Comparing `tmp/embykeeper-2.1.0.tar.gz` & `tmp/embykeeper-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.1.0.tar", last modified: Sun May 21 21:04:36 2023, max compression
+gzip compressed data, was "embykeeper-2.1.1.tar", last modified: Tue Jun 13 09:11:16 2023, max compression
```

## Comparing `embykeeper-2.1.0.tar` & `embykeeper-2.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.032250 embykeeper-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 21:04:25.000000 embykeeper-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-05-21 21:04:36.032250 embykeeper-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19758 2023-05-21 21:04:25.000000 embykeeper-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.020250 embykeeper-2.1.0/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.024250 embykeeper-2.1.0/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.024250 embykeeper-2.1.0/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.028250 embykeeper-2.1.0/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.028250 embykeeper-2.1.0/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.032250 embykeeper-2.1.0/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13927 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.024250 embykeeper-2.1.0/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:04:35.000000 embykeeper-2.1.0/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-21 21:04:25.000000 embykeeper-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:04:36.032250 embykeeper-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.032250 embykeeper-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-21 21:04:25.000000 embykeeper-2.1.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.731705 embykeeper-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 09:11:04.000000 embykeeper-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-06-13 09:11:16.731705 embykeeper-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-06-13 09:11:04.000000 embykeeper-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.731705 embykeeper-2.1.1/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-13 09:11:04.000000 embykeeper-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:11:16.731705 embykeeper-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.731705 embykeeper-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-13 09:11:04.000000 embykeeper-2.1.1/tests/test_cli.py
```

### Comparing `embykeeper-2.1.0/LICENSE` & `embykeeper-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/PKG-INFO` & `embykeeper-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.1.0
+Version: 2.1.1
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -193,14 +193,20 @@
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
 恭喜您！您已经成功部署了 Embykeeper.
 
+当您需要更新版本时, 您需要执行:
+
+```bash
+docker pull embykeeper/embykeeper
+```
+
 ### 通过 Docker Compose 部署
 
 您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
 
 **注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
 
 您需要新建一个文件 `docker-compose.yml`:
@@ -219,15 +225,15 @@
     container_name: watchtower
     image: containrrr/watchtower
     restart: unless-stopped
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务.
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
 
 然后运行以下命令以启动:
 
 ```bash
 docker-compose up -d
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.1.0 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.1.1 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
 :: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
@@ -129,34 +129,34 @@
 å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
 embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
 æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
 net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
 ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ### éè¿ Docker Compose
-é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/
-) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker é¨ç½²]
-(https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2)
-æè½éè¿ `docker-compose` é¨ç½²,
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
+æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
+Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
+compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker
+é¨ç½²](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-
+%E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
-watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡.
-ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨: ```bash docker-compose up -d ```
-å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -f embykeeper`
-æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿. ##
-å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash
-$ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
-æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
+```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
+æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
+f embykeeper` ä»¥æ¥çææ°æ¥å¿. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡
+`embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨
+Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
 (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
 (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
 e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
```

### Comparing `embykeeper-2.1.0/README.md` & `embykeeper-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,20 @@
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
 恭喜您！您已经成功部署了 Embykeeper.
 
+当您需要更新版本时, 您需要执行:
+
+```bash
+docker pull embykeeper/embykeeper
+```
+
 ### 通过 Docker Compose 部署
 
 您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
 
 **注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
 
 您需要新建一个文件 `docker-compose.yml`:
@@ -199,15 +205,15 @@
     container_name: watchtower
     image: containrrr/watchtower
     restart: unless-stopped
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务.
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
 
 然后运行以下命令以启动:
 
 ```bash
 docker-compose up -d
 ```
```

#### html2text {}

```diff
@@ -118,34 +118,34 @@
 å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
 embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
 æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
 net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
 ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ### éè¿ Docker Compose
-é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/
-) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker é¨ç½²]
-(https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2)
-æè½éè¿ `docker-compose` é¨ç½²,
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
+æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
+Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
+compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker
+é¨ç½²](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-
+%E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
-watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡.
-ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨: ```bash docker-compose up -d ```
-å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -f embykeeper`
-æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿. ##
-å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash
-$ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
-æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
+```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
+æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
+f embykeeper` ä»¥æ¥çææ°æ¥å¿. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡
+`embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨
+Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
 (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
 (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
 e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
```

### Comparing `embykeeper-2.1.0/embykeeper/cli.py` & `embykeeper-2.1.1/embykeeper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     ),
     monitor: bool = typer.Option(False, "--monitor", "-m", rich_help_panel="模块开关", help="启用群聊监视"),
     send: bool = typer.Option(False, "--send", "-s", rich_help_panel="模块开关", help="启用自动水群"),
     instant: bool = typer.Option(
         True, "--instant/--no-instant", "-i/-I", rich_help_panel="调试参数", help="立刻执行一次任务"
     ),
     once: bool = typer.Option(False, "--once/--cron", "-o/-O", rich_help_panel="调试参数", help="仅执行一次任务而不计划执行"),
+    public: bool = typer.Option(False, rich_help_panel="调试参数", help="启用公共仓库部署模式"),
     debug: bool = typer.Option(False, "--debug", "-d", rich_help_panel="调试参数", help="开启调试模式"),
     debug_cron: bool = typer.Option(False, hidden=True, help="开启任务调试模式, 在三秒后立刻开始执行计划任务"),
     version: bool = typer.Option(
         None,
         "--version",
         "-v",
         rich_help_panel="调试参数",
@@ -75,15 +76,15 @@
     analyze: bool = typer.Option(False, "--analyze", "-a", rich_help_panel="调试参数", help="仅启动历史信息分析"),
     basedir: Path = typer.Option(None, rich_help_panel="调试参数", help="设定输出文件位置"),
 ):
     from .log import logger, initialize
 
     initialize(level="DEBUG" if debug else "INFO")
 
-    config: dict = prepare_config(config)
+    config: dict = prepare_config(config, public=public)
 
     if debug:
         config["nofail"] = False
         logger.warning("您当前处于调试模式, 错误将会导致程序停止运行.")
     if debug_cron:
         logger.warning("您当前处于计划任务调试模式, 将在 3 秒后运行计划任务.")
 
@@ -121,15 +122,15 @@
         notifier,
     )
 
     if follow:
         return await follower(config)
 
     if analyze:
-        indent = " " * 29
+        indent = " " * 23
         chats = typer.prompt(indent + "请输入群组用户名 (以空格分隔)").split()
         keywords = typer.prompt(indent + "请输入关键词 (以空格分隔)", default="", show_default=False)
         keywords = keywords.split() if keywords else []
         timerange = typer.prompt(indent + '请输入时间范围 (以"-"分割)', default="", show_default=False)
         timerange = timerange.split("-") if timerange else []
         limit = typer.prompt(indent + "请输入各群组最大获取数量", default=1000, type=int)
         return await analyzer(config, chats, keywords, timerange, limit)
```

### Comparing `embykeeper-2.1.0/embykeeper/data.py` & `embykeeper-2.1.1/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/embywatcher/emby.py` & `embykeeper-2.1.1/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/embywatcher/main.py` & `embykeeper-2.1.1/embykeeper/embywatcher/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             else:
                 break
             await asyncio.sleep(10)
     except asyncio.CancelledError:
         pass
 
 
-async def play(obj: EmbyObject, time=800, progress=1000):
+async def play(obj: EmbyObject, time=10, progress=1000):
     c: Connector = obj.connector
     # 检查
     if obj.object_dict.get("RunTimeTicks") < max(progress, time) * 10000000:
         raise PlayError("视频长度低于观看进度所需")
     # 获取播放源
     resp = await c.postJson(f"/Items/{obj.id}/PlaybackInfo", isPlayBack=True, AutoOpenLiveStream=True)
     if not resp["MediaSources"]:
@@ -122,15 +122,15 @@
             info = await emby.info()
         except (ConnectionError, RuntimeError, ClientConnectionError):
             logger.error(f'Emby ({a["url"]}) 连接错误, 请重新检查配置.')
             continue
         if info:
             loggeruser = logger.bind(server=info["ServerName"], username=a["username"])
             loggeruser.info(f'成功登录 ({"Jellyfin" if a.get("jellyfin", False) else "Emby"} {info["Version"]}).')
-            yield emby, a.get("time", 800), a.get("progress", 1000), loggeruser
+            yield emby, a.get("time", 10), a.get("progress", 1000), loggeruser
         else:
             logger.error(f'Emby ({a["url"]}) 无法获取元信息而跳过, 请重新检查配置.')
             continue
 
 
 async def watch(emby, time, progress, logger, retries=5):
     retry = 0
```

### Comparing `embykeeper-2.1.0/embykeeper/log.py` & `embykeeper-2.1.1/embykeeper/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
 def initialize(level="INFO"):
     logger.remove()
     handler = RichHandler(
         console=Console(stderr=True), markup=True, rich_tracebacks=True, tracebacks_suppress=[asyncio]
     )
     handler.setFormatter(Formatter(None, "[%m/%d %H:%M]"))
-    logger.add(handler, format=formatter, level=level, colorize=False)
+    logger.add(handler, format=formatter, level=level, colorize=False, enqueue=True)
```

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/bots/base.py` & `embykeeper-2.1.1/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.1.1/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.1.1/embykeeper/telechecker/bots/jms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import asyncio
+import random
 from pyrogram.types import Message
 from thefuzz import process, fuzz
 
 from ...data import get_data
 from .base import AnswerBotCheckin
 
 __ignore__ = True
@@ -11,14 +13,15 @@
     ocr = "idioms@v1"
     idioms = None
 
     name = "卷毛鼠"
     bot_username = "jmsembybot"
 
     async def start(self):
+        self.retries = 2
         async with self.lock:
             if self.idioms is None:
                 with open(
                     await get_data(self.basedir, "idioms@v1.txt", proxy=self.proxy, caller=self.name)
                 ) as f:
                     self.__class__.idioms = [i for i in f.read().splitlines() if len(i) == 4]
         return await super().start()
@@ -36,11 +39,12 @@
         captcha = self.to_idiom(captcha)
         async with self.operable:
             if not self.message:
                 await self.operable.wait()
             for l in captcha:
                 try:
                     await self.message.click(l)
+                    await asyncio.sleep(random.randint(50, 300) / 100)
                 except ValueError:
                     self.log.info(f'未能找到对应 "{l}" 的按键, 正在重试.')
                     await self.retry()
                     break
```

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.1.1/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.1.1/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.1.1/embykeeper/telechecker/bots/pornemby.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,9 +20,9 @@
         try:
             await message.click(0)
         except TimeoutError:
             pass
         try:
             msg = await self.client.wait_reply(self.bot_username, timeout=10)
         except asyncio.TimeoutError:
-            self.log.warning(f"签到无回应, 您可能还没有注册{self.name}.")
+            self.log.warning(f"签到失败: 签到无回应, 您可能还没有注册{self.name}.")
             await self.fail()
```

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.1.1/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/link.py` & `embykeeper-2.1.1/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/log.py` & `embykeeper-2.1.1/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/main.py` & `embykeeper-2.1.1/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/messager/base.py` & `embykeeper-2.1.1/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/messager/common.py` & `embykeeper-2.1.1/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.1.1/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.1.1/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.1.1/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.1.1/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.1.1/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.1.1/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.1.1/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.1.1/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/embykeeper/telechecker/tele.py` & `embykeeper-2.1.1/embykeeper/telechecker/tele.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,17 @@
                     SentCodeType.CALL: "来电",
                     SentCodeType.FLASH_CALL: "闪存呼叫",
                     SentCodeType.FRAGMENT_SMS: "Fragment短信",
                     SentCodeType.EMAIL_CODE: "邮件",
                 }
                 if not self.phone_code:
                     if retry:
-                        msg = f'验证码错误, 请重新输入 "{self.phone_number}" 的登录验证码'
+                        msg = f'验证码错误, 请重新输入 "{self.phone_number}" 的登录验证码 (按回车确认)'
                     else:
-                        msg = f'请从{code_target[sent_code.type]}接收 "{self.phone_number}" 的登录验证码'
+                        msg = f'请从{code_target[sent_code.type]}接收 "{self.phone_number}" 的登录验证码 (按回车确认)'
                     self.phone_code = Prompt.ask(" " * 23 + msg)
                 signed_in = await self.sign_in(self.phone_number, sent_code.phone_code_hash, self.phone_code)
             except (CodeInvalid, PhoneCodeInvalid):
                 self.phone_code = None
                 retry = True
             except SessionPasswordNeeded:
                 retry = False
@@ -306,15 +306,15 @@
                         proxy=proxy,
                         lang_code="zh",
                         workdir=self.basedir,
                     )
                     await client.start()
                 except Unauthorized:
                     await client.storage.delete()
-                except KeyError:
+                except KeyError as e:
                     logger.warning(f'登录账号 "{client.phone_number}" 时发生异常, 可能是由于网络错误, 将在 3 秒后重试.')
                     await asyncio.sleep(3)
                 else:
                     break
         except asyncio.CancelledError:
             raise
         except RPCError as e:
```

### Comparing `embykeeper-2.1.0/embykeeper/utils.py` & `embykeeper-2.1.1/embykeeper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,21 @@
         def decorator(async_func):
             @wraps(async_func)
             def sync_func(*_args, **_kwargs):
                 try:
                     asyncio.run(async_func(*_args, **_kwargs))
                 except KeyboardInterrupt:
                     print("\r", end="", flush=True)
-                    logger.info("所有客户端已停止, 欢迎您再次使用 Embykeeper.")
+                    logger.info(f"所有客户端已停止, 欢迎您再次使用 {__name__.capitalize()}.")
                 except Exception as e:
                     print("\r", end="", flush=True)
                     fail_message(e)
                     sys.exit(1)
                 else:
-                    logger.info("所有任务已完成, 欢迎您再次使用 Embykeeper.")
+                    logger.info(f"所有任务已完成, 欢迎您再次使用 {__name__.capitalize()}.")
 
             self.command(*args, **kwargs)(sync_func)
             return async_func
 
         return decorator
```

### Comparing `embykeeper-2.1.0/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.1.1/embykeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.1.0
+Version: 2.1.1
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -193,14 +193,20 @@
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
 恭喜您！您已经成功部署了 Embykeeper.
 
+当您需要更新版本时, 您需要执行:
+
+```bash
+docker pull embykeeper/embykeeper
+```
+
 ### 通过 Docker Compose 部署
 
 您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
 
 **注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
 
 您需要新建一个文件 `docker-compose.yml`:
@@ -219,15 +225,15 @@
     container_name: watchtower
     image: containrrr/watchtower
     restart: unless-stopped
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务.
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
 
 然后运行以下命令以启动:
 
 ```bash
 docker-compose up -d
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.1.0 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.1.1 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
 :: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
@@ -129,34 +129,34 @@
 å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
 embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
 æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
 net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
 ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ### éè¿ Docker Compose
-é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/
-) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker é¨ç½²]
-(https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2)
-æè½éè¿ `docker-compose` é¨ç½²,
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
+æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
+Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
+compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker
+é¨ç½²](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-
+%E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
-watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡.
-ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨: ```bash docker-compose up -d ```
-å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -f embykeeper`
-æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿. ##
-å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash
-$ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
-æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
+```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
+æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
+f embykeeper` ä»¥æ¥çææ°æ¥å¿. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡
+`embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨
+Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
 (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
 (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
 e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
```

### Comparing `embykeeper-2.1.0/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.1.1/embykeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.0/pyproject.toml` & `embykeeper-2.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
@@ -47,14 +47,15 @@
     "pyrogram",
     "tgcrypto",
     "pillow",
     "thefuzz[speedup]",
     "schema",
     "aiocache",
     "fake_useragent",
+    "pycryptodome"
 ]
 
 [project.urls]
 Homepage = "https://github.com/embykeeper/embykeeper"
 
 [project.readme]
 file = "README.md"
```

### Comparing `embykeeper-2.1.0/tests/test_cli.py` & `embykeeper-2.1.1/tests/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,78 @@
 import os
 from pathlib import Path
 from typer.testing import CliRunner
 
 import tomli as tomllib
-import tomlkit
 import pytest
+import tomlkit
 
 import embykeeper
 from embykeeper.cli import app
 from embykeeper.settings import check_config
 
-runner = CliRunner(mix_stderr=False)
+runner = CliRunner()
 
 
 @pytest.fixture()
 def in_temp_dir(tmp_path: Path):
     current = os.getcwd()
     os.chdir(tmp_path)
     yield tmp_path
     os.chdir(current)
 
 
-@pytest.fixture()
-def generated_config(in_temp_dir: Path):
-    runner.invoke(app)
-
-
 def test_version():
     result = runner.invoke(app, ["--version"])
     assert embykeeper.__version__ in result.stdout
     assert result.exit_code == 0
 
 
 def test_create_config(in_temp_dir: Path):
     result = runner.invoke(app)
-    print(result.stderr)
-    assert "生成" in result.stderr
     assert result.exit_code == 250
     assert Path("config.toml").exists()
     with open("config.toml", "rb") as f:
         config = tomllib.load(f)
     assert not check_config(config)
 
 
 def test_create_config_empty(in_temp_dir: Path):
     config_file = Path("config.toml")
     config_file.touch()
     result = runner.invoke(app, [str(config_file)])
-    print(result.stderr)
-    assert "生成" in result.stderr
     assert result.exit_code == 250
     with open("config.toml", "rb") as f:
         config = tomllib.load(f)
     assert config
 
     config_file.unlink()
     config_file.touch()
     result = runner.invoke(app)
-    print(result.stderr)
-    assert "生成" in result.stderr
     assert result.exit_code == 250
     with open("config.toml", "rb") as f:
         config = tomllib.load(f)
     assert config
 
     config_file = Path("empty.toml")
     config_file.touch()
     result = runner.invoke(app, [str(config_file), "--once"])
-    assert "生成" not in result.stderr
     assert result.exit_code == 0
 
 
 def test_nonexist_config(in_temp_dir: Path):
     for fn in ("config.toml", "nonexisting.toml"):
         result = runner.invoke(app, [fn])
-        print(result.stderr)
-        assert "不存在" in result.stderr
         assert result.exit_code == 251
 
 
 def test_check_config(in_temp_dir: Path):
     with open("config.toml", "w+") as f:
         f.write("notifier: true")
     result = runner.invoke(app)
-    print(result.stderr)
-    assert "配置文件错误" in result.stderr
     assert result.exit_code == 252
 
     config = {"telegram": {k: "Test" for k in ("api_id", "api_hash", "phone")}}
     with open("config.toml", "w+") as f:
         tomlkit.dump(config, f)
     result = runner.invoke(app)
-    print(result.stderr)
-    assert "配置文件错误" in result.stderr
     assert result.exit_code == 253
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

