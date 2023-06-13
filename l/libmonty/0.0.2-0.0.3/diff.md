# Comparing `tmp/libmonty-0.0.2.tar.gz` & `tmp/libmonty-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmonty-0.0.2.tar", last modified: Mon Jan 24 20:02:24 2022, max compression
+gzip compressed data, was "libmonty-0.0.3.tar", last modified: Tue Jun 13 11:03:18 2023, max compression
```

## Comparing `libmonty-0.0.2.tar` & `libmonty-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,70 @@
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.813389 libmonty-0.0.2/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    16725 2021-12-20 00:21:09.000000 libmonty-0.0.2/LICENSE
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       37 2021-12-20 04:31:34.000000 libmonty-0.0.2/MANIFEST.in
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1766 2022-01-24 20:02:24.813389 libmonty-0.0.2/PKG-INFO
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      863 2022-01-12 02:59:23.000000 libmonty-0.0.2/README.md
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      104 2021-12-16 04:36:50.000000 libmonty-0.0.2/pyproject.toml
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1194 2022-01-24 20:02:24.813389 libmonty-0.0.2/setup.cfg
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.805389 libmonty-0.0.2/src/
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.805389 libmonty-0.0.2/src/libmonty/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:31:14.000000 libmonty-0.0.2/src/libmonty/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1509 2021-12-20 07:17:27.000000 libmonty-0.0.2/src/libmonty/__main__.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.805389 libmonty-0.0.2/src/libmonty/data/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      536 2021-12-20 04:31:34.000000 libmonty-0.0.2/src/libmonty/data/logger.ini
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.809389 libmonty-0.0.2/src/libmonty/environment/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.2/src/libmonty/environment/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      575 2021-12-20 00:53:31.000000 libmonty-0.0.2/src/libmonty/environment/terminal.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.809389 libmonty-0.0.2/src/libmonty/filesystem/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.2/src/libmonty/filesystem/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1797 2022-01-24 20:01:35.000000 libmonty-0.0.2/src/libmonty/filesystem/copy_stubs.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3264 2021-12-20 04:06:40.000000 libmonty-0.0.2/src/libmonty/filesystem/directory.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.809389 libmonty-0.0.2/src/libmonty/formatting/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.2/src/libmonty/formatting/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1390 2021-12-20 00:53:31.000000 libmonty-0.0.2/src/libmonty/formatting/char_str.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      754 2021-12-20 04:06:40.000000 libmonty-0.0.2/src/libmonty/formatting/debugging.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1338 2021-12-20 00:53:31.000000 libmonty-0.0.2/src/libmonty/formatting/json.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2147 2021-12-20 04:06:40.000000 libmonty-0.0.2/src/libmonty/formatting/number_str.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.813389 libmonty-0.0.2/src/libmonty/images/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.2/src/libmonty/images/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4206 2021-12-20 04:06:39.000000 libmonty-0.0.2/src/libmonty/images/colors_named.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1068 2021-12-20 04:06:40.000000 libmonty-0.0.2/src/libmonty/images/convert_from_stream.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.813389 libmonty-0.0.2/src/libmonty/network/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.2/src/libmonty/network/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    36448 2021-12-20 04:06:40.000000 libmonty-0.0.2/src/libmonty/network/responses.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.813389 libmonty-0.0.2/src/libmonty/outpututils/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.2/src/libmonty/outpututils/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4853 2021-12-20 04:06:40.000000 libmonty-0.0.2/src/libmonty/outpututils/asciistyling.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     5179 2021-12-20 06:35:07.000000 libmonty-0.0.2/src/libmonty/outpututils/decorators.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      318 2021-12-20 12:51:58.000000 libmonty-0.0.2/src/libmonty/version.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2022-01-24 20:02:24.805389 libmonty-0.0.2/src/libmonty.egg-info/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1766 2022-01-24 20:02:24.000000 libmonty-0.0.2/src/libmonty.egg-info/PKG-INFO
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      999 2022-01-24 20:02:24.000000 libmonty-0.0.2/src/libmonty.egg-info/SOURCES.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        1 2022-01-24 20:02:24.000000 libmonty-0.0.2/src/libmonty.egg-info/dependency_links.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      111 2022-01-24 20:02:24.000000 libmonty-0.0.2/src/libmonty.egg-info/entry_points.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        9 2022-01-24 20:02:24.000000 libmonty-0.0.2/src/libmonty.egg-info/top_level.txt
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.528770 libmonty-0.0.3/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    16725 2021-12-20 00:21:09.000000 libmonty-0.0.3/LICENSE
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        2 2023-06-12 05:01:39.000000 libmonty-0.0.3/MANIFEST.in
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1913 2023-06-13 11:03:18.528770 libmonty-0.0.3/PKG-INFO
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      954 2023-06-13 10:43:12.000000 libmonty-0.0.3/README.md
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      104 2021-12-16 04:36:50.000000 libmonty-0.0.3/pyproject.toml
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       77 2023-06-12 04:35:21.000000 libmonty-0.0.3/requirements.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1570 2023-06-13 11:03:18.528770 libmonty-0.0.3/setup.cfg
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.504770 libmonty-0.0.3/src/
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.508770 libmonty-0.0.3/src/libmonty/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:31:14.000000 libmonty-0.0.3/src/libmonty/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1241 2023-06-12 05:33:33.000000 libmonty-0.0.3/src/libmonty/__main__.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.508770 libmonty-0.0.3/src/libmonty/environment/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/environment/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      575 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/environment/terminal.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.508770 libmonty-0.0.3/src/libmonty/fileformats/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-25 12:40:19.000000 libmonty-0.0.3/src/libmonty/fileformats/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    10020 2022-09-25 13:21:40.000000 libmonty-0.0.3/src/libmonty/fileformats/oab_process.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.512770 libmonty-0.0.3/src/libmonty/filesystem/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/filesystem/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1797 2022-01-24 20:01:35.000000 libmonty-0.0.3/src/libmonty/filesystem/copy_stubs.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3264 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/filesystem/directory.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3845 2022-09-23 23:06:46.000000 libmonty-0.0.3/src/libmonty/filesystem/tree_exec.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.512770 libmonty-0.0.3/src/libmonty/formatting/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/formatting/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1390 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/formatting/char_str.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      754 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/formatting/debugging.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1338 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/formatting/json.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2147 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/formatting/number_str.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.512770 libmonty-0.0.3/src/libmonty/images/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.3/src/libmonty/images/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4206 2021-12-20 04:06:39.000000 libmonty-0.0.3/src/libmonty/images/colors_named.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1068 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/images/convert_from_stream.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.516770 libmonty-0.0.3/src/libmonty/network/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.3/src/libmonty/network/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    36448 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/network/responses.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.516770 libmonty-0.0.3/src/libmonty/outpututils/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.3/src/libmonty/outpututils/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4853 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/outpututils/asciistyling.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     5179 2021-12-20 06:35:07.000000 libmonty-0.0.3/src/libmonty/outpututils/decorators.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      580 2022-10-02 12:32:54.000000 libmonty-0.0.3/src/libmonty/outpututils/discord.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.520770 libmonty-0.0.3/src/libmonty/sound/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-23 22:47:02.000000 libmonty-0.0.3/src/libmonty/sound/__init__.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.520770 libmonty-0.0.3/src/libmonty/sound/formats/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty/sound/formats/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    12704 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty/sound/formats/wave_pcm.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      318 2023-06-12 04:35:09.000000 libmonty-0.0.3/src/libmonty/version.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.508770 libmonty-0.0.3/src/libmonty.egg-info/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1913 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/PKG-INFO
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1845 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/SOURCES.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        1 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/dependency_links.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      222 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/entry_points.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       69 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/requires.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       47 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/top_level.txt
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.520770 libmonty-0.0.3/src/libmonty_easypass/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-24 21:02:31.000000 libmonty-0.0.3/src/libmonty_easypass/__init__.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.524770 libmonty-0.0.3/src/libmonty_easypass/data/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    87335 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/agr-wordlist-en-alt-edited-by-alan-beale.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    87393 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/agr-wordlist-en-original.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)   108800 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/eff-large-wordlist.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    13660 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/eff-short-wordlist-1.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    17258 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/eff-short-wordlist-2-0.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1737 2022-09-24 22:16:34.000000 libmonty-0.0.3/src/libmonty_easypass/dice_methods.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     5861 2022-09-25 01:05:57.000000 libmonty-0.0.3/src/libmonty_easypass/easypass.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.528770 libmonty-0.0.3/src/libmonty_soundboard/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty_soundboard/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2441 2023-06-12 05:34:18.000000 libmonty-0.0.3/src/libmonty_soundboard/__main__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1496 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty_soundboard/config.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1323 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty_soundboard/sound.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      329 2023-06-12 04:43:03.000000 libmonty-0.0.3/src/libmonty_soundboard/version.py
```

### Comparing `libmonty-0.0.2/LICENSE` & `libmonty-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/PKG-INFO` & `libmonty-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmonty
-Version: 0.0.2
+Version: 0.0.3
 Summary: libmonty - a collection of Python tools
 Home-page: https://github.com/sunarch/libmonty
 Author: András Németh (sunarch)
 Author-email: sunarch@protonmail.com
 Maintainer: András Németh (sunarch)
 Maintainer-email: sunarch@protonmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
@@ -14,23 +14,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
+Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libmonty - Python libraries
 
 Python libraries
 
+## parts
+
+- [libmonty-easypass](easypass.md)
+    - a passphrase generation tool
+
 ## Installation
 
 The package is on PyPI: [libmonty](https://pypi.org/project/libmonty/)
 
 ```
 pip install libmonty
 ```
@@ -43,11 +49,14 @@
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at http://mozilla.org/MPL/2.0/.
 ```
 
 ## Acknowledgements
 
-- Python section in global .gitignore taken from [github/gitignore](https://github.com/github/gitignore) under the [CC0-1.0 License](https://choosealicense.com/licenses/cc0-1.0/).
-- Thanks to [Guido van Rossum](https://gvanrossum.github.io/), the [Python Software Foundation](https://www.python.org/psf/), and all contributors for the [Python](https://www.python.org/) programming language
-
-
+- Python section in global .gitignore taken from
+  [github/gitignore](https://github.com/github/gitignore) under the
+  [CC0-1.0 License](https://choosealicense.com/licenses/cc0-1.0/).
+- Thanks to [Guido van Rossum](https://gvanrossum.github.io/),
+  the [Python Software Foundation](https://www.python.org/psf/),
+  and all contributors for the [Python](https://www.python.org/)
+  programming language
```

### Comparing `libmonty-0.0.2/README.md` & `libmonty-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # libmonty - Python libraries
 
 Python libraries
 
+## parts
+
+- [libmonty-easypass](easypass.md)
+    - a passphrase generation tool
+
 ## Installation
 
 The package is on PyPI: [libmonty](https://pypi.org/project/libmonty/)
 
 ```
 pip install libmonty
 ```
@@ -18,9 +23,14 @@
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at http://mozilla.org/MPL/2.0/.
 ```
 
 ## Acknowledgements
 
-- Python section in global .gitignore taken from [github/gitignore](https://github.com/github/gitignore) under the [CC0-1.0 License](https://choosealicense.com/licenses/cc0-1.0/).
-- Thanks to [Guido van Rossum](https://gvanrossum.github.io/), the [Python Software Foundation](https://www.python.org/psf/), and all contributors for the [Python](https://www.python.org/) programming language
+- Python section in global .gitignore taken from
+  [github/gitignore](https://github.com/github/gitignore) under the
+  [CC0-1.0 License](https://choosealicense.com/licenses/cc0-1.0/).
+- Thanks to [Guido van Rossum](https://gvanrossum.github.io/),
+  the [Python Software Foundation](https://www.python.org/psf/),
+  and all contributors for the [Python](https://www.python.org/)
+  programming language
```

### Comparing `libmonty-0.0.2/setup.cfg` & `libmonty-0.0.3/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -12,36 +12,45 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 	Operating System :: OS Independent
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	Intended Audience :: End Users/Desktop
 	Topic :: Utilities
+	Topic :: Multimedia :: Sound/Audio :: Players
 	Typing :: Typed
 license = Mozilla Public License 2.0 (MPL 2.0)
 description = libmonty - a collection of Python tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = libmonty
 platforms = Any
 
 [options]
+install_requires = file: requirements.txt
 python_requires = >=3.9
 packages = find:
 package_dir = 
 	= src
 
 [options.entry_points]
 console_scripts = 
 	libmonty = libmonty.__main__:main
 	libmonty-copy-stubs = libmonty.filesystem.copy_stubs:main
+	libmonty-tree-exec = libmonty.filesystem.tree_exec:main
+	libmonty-soundboard = libmonty_soundboard.__main__:main
 
 [options.packages.find]
 where = src
 
 [options.package_data]
-libmonty = data/logger.ini
+libmonty_easypass = 
+	data/agr-wordlist-en-original.txt
+	data/agr-wordlist-en-alt-edited-by-alan-beale.txt
+	data/eff-large-wordlist.txt
+	data/eff-short-wordlist-1.txt
+	data/eff-short-wordlist-2-0.txt
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `libmonty-0.0.2/src/libmonty/environment/terminal.py` & `libmonty-0.0.3/src/libmonty/environment/terminal.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/filesystem/copy_stubs.py` & `libmonty-0.0.3/src/libmonty/filesystem/copy_stubs.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/filesystem/directory.py` & `libmonty-0.0.3/src/libmonty/filesystem/directory.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/formatting/char_str.py` & `libmonty-0.0.3/src/libmonty/formatting/char_str.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/formatting/debugging.py` & `libmonty-0.0.3/src/libmonty/formatting/debugging.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/formatting/json.py` & `libmonty-0.0.3/src/libmonty/formatting/json.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/formatting/number_str.py` & `libmonty-0.0.3/src/libmonty/formatting/number_str.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/images/colors_named.py` & `libmonty-0.0.3/src/libmonty/images/colors_named.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/images/convert_from_stream.py` & `libmonty-0.0.3/src/libmonty/images/convert_from_stream.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/network/responses.py` & `libmonty-0.0.3/src/libmonty/network/responses.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/outpututils/asciistyling.py` & `libmonty-0.0.3/src/libmonty/outpututils/asciistyling.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty/outpututils/decorators.py` & `libmonty-0.0.3/src/libmonty/outpututils/decorators.py`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.2/src/libmonty.egg-info/PKG-INFO` & `libmonty-0.0.3/src/libmonty.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmonty
-Version: 0.0.2
+Version: 0.0.3
 Summary: libmonty - a collection of Python tools
 Home-page: https://github.com/sunarch/libmonty
 Author: András Németh (sunarch)
 Author-email: sunarch@protonmail.com
 Maintainer: András Németh (sunarch)
 Maintainer-email: sunarch@protonmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
@@ -14,23 +14,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
+Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libmonty - Python libraries
 
 Python libraries
 
+## parts
+
+- [libmonty-easypass](easypass.md)
+    - a passphrase generation tool
+
 ## Installation
 
 The package is on PyPI: [libmonty](https://pypi.org/project/libmonty/)
 
 ```
 pip install libmonty
 ```
@@ -43,11 +49,14 @@
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at http://mozilla.org/MPL/2.0/.
 ```
 
 ## Acknowledgements
 
-- Python section in global .gitignore taken from [github/gitignore](https://github.com/github/gitignore) under the [CC0-1.0 License](https://choosealicense.com/licenses/cc0-1.0/).
-- Thanks to [Guido van Rossum](https://gvanrossum.github.io/), the [Python Software Foundation](https://www.python.org/psf/), and all contributors for the [Python](https://www.python.org/) programming language
-
-
+- Python section in global .gitignore taken from
+  [github/gitignore](https://github.com/github/gitignore) under the
+  [CC0-1.0 License](https://choosealicense.com/licenses/cc0-1.0/).
+- Thanks to [Guido van Rossum](https://gvanrossum.github.io/),
+  the [Python Software Foundation](https://www.python.org/psf/),
+  and all contributors for the [Python](https://www.python.org/)
+  programming language
```

