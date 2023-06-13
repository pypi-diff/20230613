# Comparing `tmp/fb_tools-2.2.3.tar.gz` & `tmp/fb_tools-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_tools-2.2.3.tar", last modified: Wed May 31 15:59:53 2023, max compression
+gzip compressed data, was "fb_tools-2.2.4.tar", last modified: Tue Jun 13 10:26:17 2023, max compression
```

## Comparing `fb_tools-2.2.3.tar` & `fb_tools-2.2.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.764640 fb_tools-2.2.3/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-05-31 15:59:30.000000 fb_tools-2.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2023-05-31 15:59:30.000000 fb_tools-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-31 15:59:53.764640 fb_tools-2.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-31 15:59:30.000000 fb_tools-2.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.756640 fb_tools-2.2.3/bin/
--rwxr-xr-x   0 root         (0) root         (0)     2463 2023-05-31 15:59:30.000000 fb_tools-2.2.3/bin/get-file-to-remove
--rwxr-xr-x   0 root         (0) root         (0)     1574 2023-05-31 15:59:30.000000 fb_tools-2.2.3/bin/myip
--rwxr-xr-x   0 root         (0) root         (0)     1588 2023-05-31 15:59:30.000000 fb_tools-2.2.3/bin/update-ddns
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.756640 fb_tools-2.2.3/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/lib/fb_tools/
--rw-r--r--   0 root         (0) root         (0)      406 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28061 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/app.py
--rw-r--r--   0 root         (0) root         (0)     8423 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/argparse_actions.py
--rw-r--r--   0 root         (0) root         (0)     9654 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/cfg_app.py
--rw-r--r--   0 root         (0) root         (0)    36990 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/collections.py
--rw-r--r--   0 root         (0) root         (0)    24990 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/common.py
--rw-r--r--   0 root         (0) root         (0)     8163 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/lib/fb_tools/ddns/
--rw-r--r--   0 root         (0) root         (0)    18917 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/ddns/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10614 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/ddns/config.py
--rw-r--r--   0 root         (0) root         (0)     5560 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/ddns/myip_app.py
--rw-r--r--   0 root         (0) root         (0)    14002 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/ddns/update_app.py
--rw-r--r--   0 root         (0) root         (0)    12591 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/errors.py
--rw-r--r--   0 root         (0) root         (0)    24492 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/get_file_rm_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/lib/fb_tools/handler/
--rw-r--r--   0 root         (0) root         (0)    14092 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43539 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/handler/lock.py
--rw-r--r--   0 root         (0) root         (0)    39509 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/handling_obj.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools/local_version.py
--rw-r--r--   0 root         (0) root         (0)    34973 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/mailaddress.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/merge.py
--rw-r--r--   0 root         (0) root         (0)    43962 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/multi_config.py
--rw-r--r--   0 root         (0) root         (0)    11761 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/obj.py
--rw-r--r--   0 root         (0) root         (0)    17133 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/pidfile.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-05-31 15:59:30.000000 fb_tools-2.2.3/lib/fb_tools/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/lib/fb_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1378 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-31 15:59:53.000000 fb_tools-2.2.3/lib/fb_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.756640 fb_tools-2.2.3/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    41697 2023-05-31 15:59:53.000000 fb_tools-2.2.3/locale/de/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    60342 2023-05-31 15:59:30.000000 fb_tools-2.2.3/locale/de/LC_MESSAGES/fb_tools.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.756640 fb_tools-2.2.3/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.760640 fb_tools-2.2.3/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5422 2023-05-31 15:59:53.000000 fb_tools-2.2.3/locale/en/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    43156 2023-05-31 15:59:30.000000 fb_tools-2.2.3/locale/en/LC_MESSAGES/fb_tools.po
--rw-r--r--   0 root         (0) root         (0)    41273 2023-05-31 15:59:30.000000 fb_tools-2.2.3/locale/fb_tools.pot
--rw-r--r--   0 root         (0) root         (0)     1795 2023-05-31 15:59:53.764640 fb_tools-2.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8889 2023-05-31 15:59:30.000000 fb_tools-2.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:59:53.764640 fb_tools-2.2.3/test/
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/call_script.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/call_sleep.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/do_sleep
--rw-r--r--   0 root         (0) root         (0)     3257 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/general.py
--rwxr-xr-x   0 root         (0) root         (0)     4459 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_00_errors.py
--rwxr-xr-x   0 root         (0) root         (0)    24389 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_05_common.py
--rwxr-xr-x   0 root         (0) root         (0)     6432 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_10_base_object.py
--rwxr-xr-x   0 root         (0) root         (0)    59500 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_13_collections.py
--rwxr-xr-x   0 root         (0) root         (0)    52741 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_15_mailaddress.py
--rwxr-xr-x   0 root         (0) root         (0)    17995 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_17_multicfg.py
--rwxr-xr-x   0 root         (0) root         (0)     5817 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_18_pidfile.py
--rwxr-xr-x   0 root         (0) root         (0)    19877 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_20_handling_object.py
--rwxr-xr-x   0 root         (0) root         (0)     7626 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_30_base_handler.py
--rwxr-xr-x   0 root         (0) root         (0)    14476 2023-05-31 15:59:30.000000 fb_tools-2.2.3/test/test_33_lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-06-13 10:25:53.000000 fb_tools-2.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-13 10:25:53.000000 fb_tools-2.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-13 10:26:17.410981 fb_tools-2.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-13 10:25:53.000000 fb_tools-2.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     2463 2023-06-13 10:25:53.000000 fb_tools-2.2.4/bin/get-file-to-remove
+-rwxr-xr-x   0 root         (0) root         (0)     1574 2023-06-13 10:25:53.000000 fb_tools-2.2.4/bin/myip
+-rwxr-xr-x   0 root         (0) root         (0)     1588 2023-06-13 10:25:53.000000 fb_tools-2.2.4/bin/update-ddns
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/lib/fb_tools/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28444 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/argparse_actions.py
+-rw-r--r--   0 root         (0) root         (0)     9654 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/cfg_app.py
+-rw-r--r--   0 root         (0) root         (0)    36990 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/collections.py
+-rw-r--r--   0 root         (0) root         (0)    24990 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/common.py
+-rw-r--r--   0 root         (0) root         (0)     8163 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/lib/fb_tools/ddns/
+-rw-r--r--   0 root         (0) root         (0)    18917 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/ddns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10614 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/ddns/config.py
+-rw-r--r--   0 root         (0) root         (0)     5590 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/ddns/myip_app.py
+-rw-r--r--   0 root         (0) root         (0)    14002 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/ddns/update_app.py
+-rw-r--r--   0 root         (0) root         (0)    12591 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/errors.py
+-rw-r--r--   0 root         (0) root         (0)    24522 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/get_file_rm_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/lib/fb_tools/handler/
+-rw-r--r--   0 root         (0) root         (0)    14092 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43539 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/handler/lock.py
+-rw-r--r--   0 root         (0) root         (0)    39509 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/handling_obj.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools/local_version.py
+-rw-r--r--   0 root         (0) root         (0)    34973 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/mailaddress.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/merge.py
+-rw-r--r--   0 root         (0) root         (0)    43962 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/multi_config.py
+-rw-r--r--   0 root         (0) root         (0)    11761 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/obj.py
+-rw-r--r--   0 root         (0) root         (0)    17133 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/pidfile.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-06-13 10:25:53.000000 fb_tools-2.2.4/lib/fb_tools/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/lib/fb_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 10:26:17.000000 fb_tools-2.2.4/lib/fb_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    41697 2023-06-13 10:26:17.000000 fb_tools-2.2.4/locale/de/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    60345 2023-06-13 10:25:53.000000 fb_tools-2.2.4/locale/de/LC_MESSAGES/fb_tools.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.406981 fb_tools-2.2.4/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5422 2023-06-13 10:26:17.000000 fb_tools-2.2.4/locale/en/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    43159 2023-06-13 10:25:53.000000 fb_tools-2.2.4/locale/en/LC_MESSAGES/fb_tools.po
+-rw-r--r--   0 root         (0) root         (0)    41282 2023-06-13 10:25:53.000000 fb_tools-2.2.4/locale/fb_tools.pot
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-13 10:26:17.414981 fb_tools-2.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8889 2023-06-13 10:25:53.000000 fb_tools-2.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:26:17.410981 fb_tools-2.2.4/test/
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/call_script.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/call_sleep.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/do_sleep
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/general.py
+-rwxr-xr-x   0 root         (0) root         (0)     4459 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_00_errors.py
+-rwxr-xr-x   0 root         (0) root         (0)    24389 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_05_common.py
+-rwxr-xr-x   0 root         (0) root         (0)     6432 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_10_base_object.py
+-rwxr-xr-x   0 root         (0) root         (0)    59500 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_13_collections.py
+-rwxr-xr-x   0 root         (0) root         (0)    52741 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_15_mailaddress.py
+-rwxr-xr-x   0 root         (0) root         (0)    17995 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_17_multicfg.py
+-rwxr-xr-x   0 root         (0) root         (0)     5817 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_18_pidfile.py
+-rwxr-xr-x   0 root         (0) root         (0)    19877 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_20_handling_object.py
+-rwxr-xr-x   0 root         (0) root         (0)     7626 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_30_base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)    14476 2023-06-13 10:25:53.000000 fb_tools-2.2.4/test/test_33_lock.py
```

### Comparing `fb_tools-2.2.3/LICENSE` & `fb_tools-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/PKG-INFO` & `fb_tools-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_tools
-Version: 2.2.3
+Version: 2.2.4
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.2.3/bin/get-file-to-remove` & `fb_tools-2.2.4/bin/get-file-to-remove`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/bin/myip` & `fb_tools-2.2.4/bin/myip`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/bin/update-ddns` & `fb_tools-2.2.4/bin/update-ddns`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/app.py` & `fb_tools-2.2.4/lib/fb_tools/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from .errors import FunctionNotImplementedError
 from .handling_obj import HandlingObject
 from .xlate import DOMAIN, LOCALE_DIR, XLATOR
 from .xlate import __base_dir__ as __xlate_base_dir__
 from .xlate import __mo_file__ as __xlate_mo_file__
 from .xlate import __module_dir__ as __xlate_module_dir__
 
-__version__ = '2.2.2'
+__version__ = '2.2.3'
 LOG = logging.getLogger(__name__)
 
 SIGNAL_NAMES = {
     signal.SIGHUP: 'HUP',
     signal.SIGINT: 'INT',
     signal.SIGABRT: 'ABRT',
     signal.SIGTERM: 'TERM',
@@ -62,14 +62,15 @@
     re_anum = re.compile(r'[^A-Z0-9_]+', re.IGNORECASE)
 
     default_force_desc_msg = _('Forced execution - whatever it means.')
 
     show_assume_options = False
     show_console_timeout_option = False
     show_force_option = False
+    show_quiet_option = True
     show_simulate_option = True
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__pkg_version__, base_dir=None, quiet=False,
             terminal_has_colors=False, simulate=None, force=None, assumed_answer=None,
             initialized=False, usage=None, description=None,
@@ -313,14 +314,15 @@
         res['description'] = self.description
         res['env_prefix'] = self.env_prefix
         res['exit_value'] = self.exit_value
         res['force_desc_msg'] = self.force_desc_msg
         res['show_assume_options'] = self.show_assume_options
         res['show_console_timeout_option'] = self.show_console_timeout_option
         res['show_force_option'] = self.show_force_option
+        res['show_quiet_option'] = self.show_quiet_option
         res['show_simulate_option'] = self.show_simulate_option
         res['usage'] = self.usage
         if 'xlate' not in res:
             res['xlate'] = {}
         res['xlate']['fb_tools'] = {
             '__module_dir__': __xlate_module_dir__,
             '__base_dir__': __xlate_base_dir__,
@@ -647,25 +649,30 @@
 
         general_group.add_argument(
             '--color', action='store', dest='color', const='yes',
             default='auto', nargs='?', choices=['yes', 'no', 'auto'],
             help=_('Use colored output for messages.'),
         )
 
-        verbose_group = general_group.add_mutually_exclusive_group()
-
-        verbose_group.add_argument(
-            '-v', '--verbose', action='count', dest='verbose',
-            help=_('Increase the verbosity level'),
-        )
-
-        verbose_group.add_argument(
-            '-q', '--quiet', action='store_true', dest='quiet',
-            help=_('Silent execution, only warnings and errors are emitted.'),
-        )
+        verbose_help = _('Increase the verbosity level')
+        if self.show_quiet_option:
+            verbose_group = general_group.add_mutually_exclusive_group()
+            verbose_group.add_argument(
+                '-v', '--verbose', action='count', dest='verbose',
+                help=verbose_help,
+            )
+            verbose_group.add_argument(
+                '-q', '--quiet', action='store_true', dest='quiet',
+                help=_('Silent execution, only warnings and errors are emitted.'),
+            )
+        else:
+            general_group.add_argument(
+                '-v', '--verbose', action='count', dest='verbose',
+                help=verbose_help,
+            )
 
         general_group.add_argument(
             '-h', '--help', action='help', dest='help',
             help=_('Show this help message and exit.')
         )
         general_group.add_argument(
             '--usage', action='store_true', dest='usage',
@@ -712,16 +719,16 @@
         if hasattr(self.args, 'assume_yes'):
             if self.args.assume_yes:
                 self.assumed_answer = True
         if hasattr(self.args, 'assume_no'):
             if self.args.assume_no:
                 self.assumed_answer = False
 
-        if self.args.quiet:
-            self.quiet = self.args.quiet
+        if hasattr(self.args, 'quiet') and self.args.quiet:
+            self.quiet = True
 
         prompt_timeout = getattr(self.args, 'console_timeout', None)
         if prompt_timeout is not None:
             self.prompt_timeout = prompt_timeout
 
         if self.args.color == 'yes':
             self._terminal_has_colors = True
```

### Comparing `fb_tools-2.2.3/lib/fb_tools/argparse_actions.py` & `fb_tools-2.2.4/lib/fb_tools/argparse_actions.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/cfg_app.py` & `fb_tools-2.2.4/lib/fb_tools/cfg_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/collections.py` & `fb_tools-2.2.4/lib/fb_tools/collections.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/common.py` & `fb_tools-2.2.4/lib/fb_tools/common.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/config.py` & `fb_tools-2.2.4/lib/fb_tools/config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/ddns/__init__.py` & `fb_tools-2.2.4/lib/fb_tools/ddns/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/ddns/config.py` & `fb_tools-2.2.4/lib/fb_tools/ddns/config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/ddns/myip_app.py` & `fb_tools-2.2.4/lib/fb_tools/ddns/myip_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 # Own modules
 from . import BaseDdnsApplication, WorkDirError
 from .config import DdnsConfiguration
 from .. import __version__ as GLOBAL_VERSION
 from ..common import to_bool
 from ..xlate import XLATOR, format_list
 
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 # =============================================================================
 class MyIpApplication(BaseDdnsApplication):
     """Class for the application objects."""
 
     show_assume_options = False
     show_console_timeout_option = False
     show_force_option = False
+    show_quiet_option = False
     show_simulate_option = False
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=GLOBAL_VERSION, base_dir=None,
             initialized=False, usage=None, description=None,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None):
```

### Comparing `fb_tools-2.2.3/lib/fb_tools/ddns/update_app.py` & `fb_tools-2.2.4/lib/fb_tools/ddns/update_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/errors.py` & `fb_tools-2.2.4/lib/fb_tools/errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/get_file_rm_app.py` & `fb_tools-2.2.4/lib/fb_tools/get_file_rm_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # Own modules
 from .app import BaseApplication
 from .common import get_monday, pp
 from .errors import FbAppError
 from .xlate import XLATOR
 
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
@@ -126,14 +126,15 @@
     min_keep_last = 1
 
     default_date_pattern = r'%Y[-_]?%m[-_]?%d'
 
     show_assume_options = False
     show_console_timeout_option = False
     show_force_option = False
+    show_quiet_option = False
     show_simulate_option = False
 
     # -------------------------------------------------------------------------
     def __init__(
             self, verbose=0, version=__version__, *arg, **kwargs):
         """Initialise of the get-file-to-remove application object."""
         desc = _(
```

### Comparing `fb_tools-2.2.3/lib/fb_tools/handler/__init__.py` & `fb_tools-2.2.4/lib/fb_tools/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/handler/lock.py` & `fb_tools-2.2.4/lib/fb_tools/handler/lock.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/handling_obj.py` & `fb_tools-2.2.4/lib/fb_tools/handling_obj.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/mailaddress.py` & `fb_tools-2.2.4/lib/fb_tools/mailaddress.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/merge.py` & `fb_tools-2.2.4/lib/fb_tools/merge.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/multi_config.py` & `fb_tools-2.2.4/lib/fb_tools/multi_config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/obj.py` & `fb_tools-2.2.4/lib/fb_tools/obj.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/pidfile.py` & `fb_tools-2.2.4/lib/fb_tools/pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools/xlate.py` & `fb_tools-2.2.4/lib/fb_tools/xlate.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/lib/fb_tools.egg-info/PKG-INFO` & `fb_tools-2.2.4/lib/fb_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-tools
-Version: 2.2.3
+Version: 2.2.4
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.2.3/lib/fb_tools.egg-info/SOURCES.txt` & `fb_tools-2.2.4/lib/fb_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/locale/de/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.2.4/locale/de/LC_MESSAGES/fb_tools.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fb_tools 2.2.3\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"POT-Creation-Date: 2023-06-13 11:48+0200\n"
 "PO-Revision-Date: 2023-05-31 17:30+0200\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: de\n"
 "Language-Team: de <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `fb_tools-2.2.3/locale/de/LC_MESSAGES/fb_tools.po` & `fb_tools-2.2.4/locale/de/LC_MESSAGES/fb_tools.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # German translations for fb_tools.
 # Copyright (C) 2023 Frank Brehm, Berlin
 # This file is distributed under the same license as the fb_tools project.
-# Frank Brehm <frank@brehm-online.com>, 2023.
+# Frank Brehm <frank.brehm@pixelpark.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: fb_tools 2.2.3\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"POT-Creation-Date: 2023-06-13 11:48+0200\n"
 "PO-Revision-Date: 2023-05-31 17:30+0200\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: de\n"
 "Language-Team: de <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -26,156 +26,156 @@
 "{c}-Objekt:\n"
 "{a}"
 
 #: lib/fb_tools/app.py:64
 msgid "Forced execution - whatever it means."
 msgstr "Forcierte Ausführung, was auch immer das bedeuten mag."
 
-#: lib/fb_tools/app.py:146
+#: lib/fb_tools/app.py:147
 msgid "Invalid env_prefix {!r} given - it may not be empty."
 msgstr "Ungültiger env_prefix {!r} übergeben - er darf nicht leer sein."
 
-#: lib/fb_tools/app.py:150
+#: lib/fb_tools/app.py:151
 msgid ""
 "Invalid characters found in env_prefix {!r}, only alphanumeric characters and digits and "
 "underscore (this not as the first character) are allowed."
 msgstr ""
 "Ungültige Zeichen in env_prefix {!r} gefunden, nur alphanumerische Zeichen und Unterstriche "
 "(diese aber nicht als erstes Zeichen) sind erlaubt."
 
-#: lib/fb_tools/app.py:161
+#: lib/fb_tools/app.py:162
 msgid "Unknown and undescriped application."
 msgstr "Unbekannte und nicht beschriebene Anwendung."
 
-#: lib/fb_tools/app.py:186
+#: lib/fb_tools/app.py:187
 msgid "Wrong exit_value {!r}, must be >= 0."
 msgstr "Falscher Wert für exit_value {!r}, muss größer als oder gleich Null sein."
 
-#: lib/fb_tools/app.py:423
+#: lib/fb_tools/app.py:425
 msgid "Trying to get {} via console ..."
 msgstr "Versuche {} über die Konsole zu bekommen …"
 
-#: lib/fb_tools/app.py:439
+#: lib/fb_tools/app.py:441
 msgid "Got a signal {}."
 msgstr "Erhielt ein Signal {}."
 
-#: lib/fb_tools/app.py:442
+#: lib/fb_tools/app.py:444
 msgid "Got a signal {n!r} ({s})."
 msgstr "Erhielt ein Signal {n!r} ({s})."
 
-#: lib/fb_tools/app.py:449
+#: lib/fb_tools/app.py:451
 msgid "Exit on signal {n!r} ({s})."
 msgstr "Beendigung auf Signal {n!r} ({s})."
 
-#: lib/fb_tools/app.py:457
+#: lib/fb_tools/app.py:459
 msgid "Tweaking signal handlers."
 msgstr "Schraube an den Signalhandlern."
 
-#: lib/fb_tools/app.py:463
+#: lib/fb_tools/app.py:465
 msgid "Setting signal handler for {n!r} ({s})."
 msgstr "Setze Signalhandler für {n!r} ({s})."
 
-#: lib/fb_tools/app.py:474
+#: lib/fb_tools/app.py:476
 msgid "Enter "
 msgstr "Eingabe von "
 
-#: lib/fb_tools/app.py:481
+#: lib/fb_tools/app.py:483
 msgid "Repeat enter "
 msgstr "Wiederholen der Eingabe von "
 
-#: lib/fb_tools/app.py:491
+#: lib/fb_tools/app.py:493
 msgid "{n} and repeated {n} did not match."
 msgstr "{n} und das wiederholte {n} stimmen nicht überein."
 
-#: lib/fb_tools/app.py:495
+#: lib/fb_tools/app.py:497
 msgid "Restoring original signal handlers."
 msgstr "Stelle original Signalhandler wieder her."
 
-#: lib/fb_tools/app.py:500
+#: lib/fb_tools/app.py:502
 msgid "Got {n!r}: {s!r}"
 msgstr "Erhielt {n!r}: {s!r}"
 
-#: lib/fb_tools/app.py:550
+#: lib/fb_tools/app.py:552
 msgid "The application is not completely initialized."
 msgstr "Die Anwendung ist nicht vollständig initialisiert."
 
-#: lib/fb_tools/app.py:561
+#: lib/fb_tools/app.py:563
 msgid "Object {!r} seems not to be completely initialized."
 msgstr "Das {!r}-Objekt scheit noch nicht vollständig initialisiert zu sein."
 
-#: lib/fb_tools/app.py:571
+#: lib/fb_tools/app.py:573
 msgid "Ending."
 msgstr "Beenden."
 
-#: lib/fb_tools/app.py:589
+#: lib/fb_tools/app.py:591
 msgid "Executing {} ..."
 msgstr "Führe {} aus …"
 
-#: lib/fb_tools/app.py:611
+#: lib/fb_tools/app.py:613
 msgid "General options"
 msgstr "Allgemeine Optionen"
 
-#: lib/fb_tools/app.py:616
+#: lib/fb_tools/app.py:618
 msgid "Simulation mode, nothing is really done."
 msgstr "Simulations-Modus, es wird nichts wirklich verändert."
 
-#: lib/fb_tools/app.py:630 lib/fb_tools/app.py:636
+#: lib/fb_tools/app.py:632 lib/fb_tools/app.py:638
 msgid "Automatically answer '{}' for all questions."
 msgstr "Automatisch alle Fragen mit {} beantworten."
 
-#: lib/fb_tools/app.py:631 lib/fb_tools/handling_obj.py:936
+#: lib/fb_tools/app.py:633 lib/fb_tools/handling_obj.py:936
 msgid "Yes"
 msgstr "Ja"
 
-#: lib/fb_tools/app.py:637 lib/fb_tools/handling_obj.py:934
+#: lib/fb_tools/app.py:639 lib/fb_tools/handling_obj.py:934
 msgid "No"
 msgstr "Nein"
 
-#: lib/fb_tools/app.py:642 lib/fb_tools/ddns/__init__.py:243
+#: lib/fb_tools/app.py:644 lib/fb_tools/ddns/__init__.py:243
 msgid "SECONDS"
 msgstr "SEKUNDEN"
 
-#: lib/fb_tools/app.py:644
+#: lib/fb_tools/app.py:646
 msgid "The timeout in seconds for console input. Default: {}"
 msgstr "Die Zeit für die Zeitüberschreitung in Sekunden für Konsolen-Eingaben Vorgabe: {}."
 
-#: lib/fb_tools/app.py:651
+#: lib/fb_tools/app.py:653
 msgid "Use colored output for messages."
 msgstr "Verwenden kolorierter Ausgabe für Mitteilungen."
 
-#: lib/fb_tools/app.py:658
+#: lib/fb_tools/app.py:656
 msgid "Increase the verbosity level"
 msgstr "Erhöhen des Ausführichkeits-Niveaus"
 
-#: lib/fb_tools/app.py:663
+#: lib/fb_tools/app.py:665
 msgid "Silent execution, only warnings and errors are emitted."
 msgstr "Stillschweigende Ausführung, nur Warnungen und Fehler werden ausgegeben."
 
-#: lib/fb_tools/app.py:668
+#: lib/fb_tools/app.py:675
 msgid "Show this help message and exit."
 msgstr "Zeigt diesen Hilfe-Bildschirm und beendet sich."
 
-#: lib/fb_tools/app.py:672
+#: lib/fb_tools/app.py:679
 msgid "Display brief usage message and exit."
 msgstr "Zeigt eine kurze Darstellug zur Verwendung und beendet sich."
 
-#: lib/fb_tools/app.py:674
+#: lib/fb_tools/app.py:681
 #, python-format
 msgid "Version of %(prog)s: {}"
 msgstr "Version von %(prog)s: {}"
 
-#: lib/fb_tools/app.py:677
+#: lib/fb_tools/app.py:684
 msgid "Show program's version number and exit."
 msgstr "Stellt die Programm-Version dar und beendet sich."
 
-#: lib/fb_tools/app.py:807
+#: lib/fb_tools/app.py:814
 msgid "Starting in:"
 msgstr "Start in:"
 
-#: lib/fb_tools/app.py:829
+#: lib/fb_tools/app.py:836
 msgid "Aborted by user interrupt."
 msgstr "Abbruch durch Benutzer-Unterbrechung."
 
 #: lib/fb_tools/argparse_actions.py:58
 msgid "Got a {c} for pattern {p!r}: {e}"
 msgstr "Habe ein(e) {c} zum Suchmuster {p!r} erhalten: {e}"
```

### Comparing `fb_tools-2.2.3/locale/en/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.2.4/locale/en/LC_MESSAGES/fb_tools.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fb_tools 2.2.3\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"POT-Creation-Date: 2023-06-13 11:48+0200\n"
 "PO-Revision-Date: 2023-05-31 17:30+0100\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: en\n"
 "Language-Team: en <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `fb_tools-2.2.3/locale/en/LC_MESSAGES/fb_tools.po` & `fb_tools-2.2.4/locale/en/LC_MESSAGES/fb_tools.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # English translations for fb_tools.
 # Copyright (C) 2023 Frank Brehm, Berlin
 # This file is distributed under the same license as the fb_tools project.
-# Frank Brehm <frank@brehm-online.com>, 2023.
+# Frank Brehm <frank.brehm@pixelpark.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: fb_tools 2.2.3\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"POT-Creation-Date: 2023-06-13 11:48+0200\n"
 "PO-Revision-Date: 2023-05-31 17:30+0100\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: en\n"
 "Language-Team: en <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -24,154 +24,154 @@
 "{a}"
 msgstr ""
 
 #: lib/fb_tools/app.py:64
 msgid "Forced execution - whatever it means."
 msgstr ""
 
-#: lib/fb_tools/app.py:146
+#: lib/fb_tools/app.py:147
 msgid "Invalid env_prefix {!r} given - it may not be empty."
 msgstr ""
 
-#: lib/fb_tools/app.py:150
+#: lib/fb_tools/app.py:151
 msgid ""
 "Invalid characters found in env_prefix {!r}, only alphanumeric characters and digits and "
 "underscore (this not as the first character) are allowed."
 msgstr ""
 
-#: lib/fb_tools/app.py:161
+#: lib/fb_tools/app.py:162
 msgid "Unknown and undescriped application."
 msgstr ""
 
-#: lib/fb_tools/app.py:186
+#: lib/fb_tools/app.py:187
 msgid "Wrong exit_value {!r}, must be >= 0."
 msgstr ""
 
-#: lib/fb_tools/app.py:423
+#: lib/fb_tools/app.py:425
 msgid "Trying to get {} via console ..."
 msgstr "Trying to get {} via console …"
 
-#: lib/fb_tools/app.py:439
+#: lib/fb_tools/app.py:441
 msgid "Got a signal {}."
 msgstr ""
 
-#: lib/fb_tools/app.py:442
+#: lib/fb_tools/app.py:444
 msgid "Got a signal {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:449
+#: lib/fb_tools/app.py:451
 msgid "Exit on signal {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:457
+#: lib/fb_tools/app.py:459
 msgid "Tweaking signal handlers."
 msgstr ""
 
-#: lib/fb_tools/app.py:463
+#: lib/fb_tools/app.py:465
 msgid "Setting signal handler for {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:474
+#: lib/fb_tools/app.py:476
 msgid "Enter "
 msgstr ""
 
-#: lib/fb_tools/app.py:481
+#: lib/fb_tools/app.py:483
 msgid "Repeat enter "
 msgstr ""
 
-#: lib/fb_tools/app.py:491
+#: lib/fb_tools/app.py:493
 msgid "{n} and repeated {n} did not match."
 msgstr ""
 
-#: lib/fb_tools/app.py:495
+#: lib/fb_tools/app.py:497
 msgid "Restoring original signal handlers."
 msgstr ""
 
-#: lib/fb_tools/app.py:500
+#: lib/fb_tools/app.py:502
 msgid "Got {n!r}: {s!r}"
 msgstr ""
 
-#: lib/fb_tools/app.py:550
+#: lib/fb_tools/app.py:552
 msgid "The application is not completely initialized."
 msgstr ""
 
-#: lib/fb_tools/app.py:561
+#: lib/fb_tools/app.py:563
 msgid "Object {!r} seems not to be completely initialized."
 msgstr ""
 
-#: lib/fb_tools/app.py:571
+#: lib/fb_tools/app.py:573
 msgid "Ending."
 msgstr ""
 
-#: lib/fb_tools/app.py:589
+#: lib/fb_tools/app.py:591
 msgid "Executing {} ..."
 msgstr "Executing {} …"
 
-#: lib/fb_tools/app.py:611
+#: lib/fb_tools/app.py:613
 msgid "General options"
 msgstr ""
 
-#: lib/fb_tools/app.py:616
+#: lib/fb_tools/app.py:618
 msgid "Simulation mode, nothing is really done."
 msgstr ""
 
-#: lib/fb_tools/app.py:630 lib/fb_tools/app.py:636
+#: lib/fb_tools/app.py:632 lib/fb_tools/app.py:638
 msgid "Automatically answer '{}' for all questions."
 msgstr ""
 
-#: lib/fb_tools/app.py:631 lib/fb_tools/handling_obj.py:936
+#: lib/fb_tools/app.py:633 lib/fb_tools/handling_obj.py:936
 msgid "Yes"
 msgstr ""
 
-#: lib/fb_tools/app.py:637 lib/fb_tools/handling_obj.py:934
+#: lib/fb_tools/app.py:639 lib/fb_tools/handling_obj.py:934
 msgid "No"
 msgstr ""
 
-#: lib/fb_tools/app.py:642 lib/fb_tools/ddns/__init__.py:243
+#: lib/fb_tools/app.py:644 lib/fb_tools/ddns/__init__.py:243
 msgid "SECONDS"
 msgstr ""
 
-#: lib/fb_tools/app.py:644
+#: lib/fb_tools/app.py:646
 msgid "The timeout in seconds for console input. Default: {}"
 msgstr ""
 
-#: lib/fb_tools/app.py:651
+#: lib/fb_tools/app.py:653
 msgid "Use colored output for messages."
 msgstr ""
 
-#: lib/fb_tools/app.py:658
+#: lib/fb_tools/app.py:656
 msgid "Increase the verbosity level"
 msgstr ""
 
-#: lib/fb_tools/app.py:663
+#: lib/fb_tools/app.py:665
 msgid "Silent execution, only warnings and errors are emitted."
 msgstr ""
 
-#: lib/fb_tools/app.py:668
+#: lib/fb_tools/app.py:675
 msgid "Show this help message and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:672
+#: lib/fb_tools/app.py:679
 msgid "Display brief usage message and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:674
+#: lib/fb_tools/app.py:681
 #, python-format
 msgid "Version of %(prog)s: {}"
 msgstr ""
 
-#: lib/fb_tools/app.py:677
+#: lib/fb_tools/app.py:684
 msgid "Show program's version number and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:807
+#: lib/fb_tools/app.py:814
 msgid "Starting in:"
 msgstr ""
 
-#: lib/fb_tools/app.py:829
+#: lib/fb_tools/app.py:836
 msgid "Aborted by user interrupt."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:58
 msgid "Got a {c} for pattern {p!r}: {e}"
 msgstr ""
```

### Comparing `fb_tools-2.2.3/locale/fb_tools.pot` & `fb_tools-2.2.4/locale/fb_tools.pot`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Translations template for fb_tools.
 # Copyright (C) 2023 Frank Brehm, Berlin
 # This file is distributed under the same license as the fb_tools project.
-# Frank Brehm <frank@brehm-online.com>, 2023.
+# Frank Brehm <frank.brehm@pixelpark.com>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: fb_tools 2.2.3\n"
-"Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"POT-Creation-Date: 2023-05-31 14:28+0200\n"
+"Report-Msgid-Bugs-To: frank.brehm@pixelpark.com\n"
+"POT-Creation-Date: 2023-06-13 11:48+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <frank@brehm-online.com>\n"
+"Last-Translator: FULL NAME <frank.brehm@pixelpark.com>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: bin/get-file-to-remove:84
@@ -23,154 +23,154 @@
 "{a}"
 msgstr ""
 
 #: lib/fb_tools/app.py:64
 msgid "Forced execution - whatever it means."
 msgstr ""
 
-#: lib/fb_tools/app.py:146
+#: lib/fb_tools/app.py:147
 msgid "Invalid env_prefix {!r} given - it may not be empty."
 msgstr ""
 
-#: lib/fb_tools/app.py:150
+#: lib/fb_tools/app.py:151
 msgid ""
 "Invalid characters found in env_prefix {!r}, only alphanumeric characters and digits and "
 "underscore (this not as the first character) are allowed."
 msgstr ""
 
-#: lib/fb_tools/app.py:161
+#: lib/fb_tools/app.py:162
 msgid "Unknown and undescriped application."
 msgstr ""
 
-#: lib/fb_tools/app.py:186
+#: lib/fb_tools/app.py:187
 msgid "Wrong exit_value {!r}, must be >= 0."
 msgstr ""
 
-#: lib/fb_tools/app.py:423
+#: lib/fb_tools/app.py:425
 msgid "Trying to get {} via console ..."
 msgstr ""
 
-#: lib/fb_tools/app.py:439
+#: lib/fb_tools/app.py:441
 msgid "Got a signal {}."
 msgstr ""
 
-#: lib/fb_tools/app.py:442
+#: lib/fb_tools/app.py:444
 msgid "Got a signal {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:449
+#: lib/fb_tools/app.py:451
 msgid "Exit on signal {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:457
+#: lib/fb_tools/app.py:459
 msgid "Tweaking signal handlers."
 msgstr ""
 
-#: lib/fb_tools/app.py:463
+#: lib/fb_tools/app.py:465
 msgid "Setting signal handler for {n!r} ({s})."
 msgstr ""
 
-#: lib/fb_tools/app.py:474
+#: lib/fb_tools/app.py:476
 msgid "Enter "
 msgstr ""
 
-#: lib/fb_tools/app.py:481
+#: lib/fb_tools/app.py:483
 msgid "Repeat enter "
 msgstr ""
 
-#: lib/fb_tools/app.py:491
+#: lib/fb_tools/app.py:493
 msgid "{n} and repeated {n} did not match."
 msgstr ""
 
-#: lib/fb_tools/app.py:495
+#: lib/fb_tools/app.py:497
 msgid "Restoring original signal handlers."
 msgstr ""
 
-#: lib/fb_tools/app.py:500
+#: lib/fb_tools/app.py:502
 msgid "Got {n!r}: {s!r}"
 msgstr ""
 
-#: lib/fb_tools/app.py:550
+#: lib/fb_tools/app.py:552
 msgid "The application is not completely initialized."
 msgstr ""
 
-#: lib/fb_tools/app.py:561
+#: lib/fb_tools/app.py:563
 msgid "Object {!r} seems not to be completely initialized."
 msgstr ""
 
-#: lib/fb_tools/app.py:571
+#: lib/fb_tools/app.py:573
 msgid "Ending."
 msgstr ""
 
-#: lib/fb_tools/app.py:589
+#: lib/fb_tools/app.py:591
 msgid "Executing {} ..."
 msgstr ""
 
-#: lib/fb_tools/app.py:611
+#: lib/fb_tools/app.py:613
 msgid "General options"
 msgstr ""
 
-#: lib/fb_tools/app.py:616
+#: lib/fb_tools/app.py:618
 msgid "Simulation mode, nothing is really done."
 msgstr ""
 
-#: lib/fb_tools/app.py:630 lib/fb_tools/app.py:636
+#: lib/fb_tools/app.py:632 lib/fb_tools/app.py:638
 msgid "Automatically answer '{}' for all questions."
 msgstr ""
 
-#: lib/fb_tools/app.py:631 lib/fb_tools/handling_obj.py:936
+#: lib/fb_tools/app.py:633 lib/fb_tools/handling_obj.py:936
 msgid "Yes"
 msgstr ""
 
-#: lib/fb_tools/app.py:637 lib/fb_tools/handling_obj.py:934
+#: lib/fb_tools/app.py:639 lib/fb_tools/handling_obj.py:934
 msgid "No"
 msgstr ""
 
-#: lib/fb_tools/app.py:642 lib/fb_tools/ddns/__init__.py:243
+#: lib/fb_tools/app.py:644 lib/fb_tools/ddns/__init__.py:243
 msgid "SECONDS"
 msgstr ""
 
-#: lib/fb_tools/app.py:644
+#: lib/fb_tools/app.py:646
 msgid "The timeout in seconds for console input. Default: {}"
 msgstr ""
 
-#: lib/fb_tools/app.py:651
+#: lib/fb_tools/app.py:653
 msgid "Use colored output for messages."
 msgstr ""
 
-#: lib/fb_tools/app.py:658
+#: lib/fb_tools/app.py:656
 msgid "Increase the verbosity level"
 msgstr ""
 
-#: lib/fb_tools/app.py:663
+#: lib/fb_tools/app.py:665
 msgid "Silent execution, only warnings and errors are emitted."
 msgstr ""
 
-#: lib/fb_tools/app.py:668
+#: lib/fb_tools/app.py:675
 msgid "Show this help message and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:672
+#: lib/fb_tools/app.py:679
 msgid "Display brief usage message and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:674
+#: lib/fb_tools/app.py:681
 #, python-format
 msgid "Version of %(prog)s: {}"
 msgstr ""
 
-#: lib/fb_tools/app.py:677
+#: lib/fb_tools/app.py:684
 msgid "Show program's version number and exit."
 msgstr ""
 
-#: lib/fb_tools/app.py:807
+#: lib/fb_tools/app.py:814
 msgid "Starting in:"
 msgstr ""
 
-#: lib/fb_tools/app.py:829
+#: lib/fb_tools/app.py:836
 msgid "Aborted by user interrupt."
 msgstr ""
 
 #: lib/fb_tools/argparse_actions.py:58
 msgid "Got a {c} for pattern {p!r}: {e}"
 msgstr ""
```

### Comparing `fb_tools-2.2.3/setup.cfg` & `fb_tools-2.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/setup.py` & `fb_tools-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/general.py` & `fb_tools-2.2.4/test/general.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_00_errors.py` & `fb_tools-2.2.4/test/test_00_errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_05_common.py` & `fb_tools-2.2.4/test/test_05_common.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_10_base_object.py` & `fb_tools-2.2.4/test/test_10_base_object.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_13_collections.py` & `fb_tools-2.2.4/test/test_13_collections.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_15_mailaddress.py` & `fb_tools-2.2.4/test/test_15_mailaddress.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_17_multicfg.py` & `fb_tools-2.2.4/test/test_17_multicfg.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_18_pidfile.py` & `fb_tools-2.2.4/test/test_18_pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_20_handling_object.py` & `fb_tools-2.2.4/test/test_20_handling_object.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_30_base_handler.py` & `fb_tools-2.2.4/test/test_30_base_handler.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.2.3/test/test_33_lock.py` & `fb_tools-2.2.4/test/test_33_lock.py`

 * *Files identical despite different names*

