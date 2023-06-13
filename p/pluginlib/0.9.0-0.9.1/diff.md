# Comparing `tmp/pluginlib-0.9.0.tar.gz` & `tmp/pluginlib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluginlib-0.9.0.tar", last modified: Sun Feb 13 21:36:48 2022, max compression
+gzip compressed data, was "pluginlib-0.9.1.tar", last modified: Tue Jun 13 01:08:07 2023, max compression
```

## Comparing `pluginlib-0.9.0.tar` & `pluginlib-0.9.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.229416 pluginlib-0.9.0/
--rw-rw-r--   0 avram     (1000) avram     (1000)    16726 2017-10-10 15:55:09.000000 pluginlib-0.9.0/LICENSE
--rw-rw-r--   0 avram     (1000) avram     (1000)       97 2022-02-13 15:53:51.000000 pluginlib-0.9.0/MANIFEST.in
--rw-rw-r--   0 avram     (1000) avram     (1000)     9598 2022-02-13 21:36:48.229416 pluginlib-0.9.0/PKG-INFO
--rw-rw-r--   0 avram     (1000) avram     (1000)     8274 2022-02-13 18:29:40.000000 pluginlib-0.9.0/README.rst
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.223416 pluginlib-0.9.0/doc/
--rw-rw-r--   0 avram     (1000) avram     (1000)     1575 2020-06-03 01:12:58.000000 pluginlib-0.9.0/doc/api.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)     8896 2018-08-28 12:21:53.000000 pluginlib-0.9.0/doc/concepts.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)     3648 2020-05-02 18:34:38.000000 pluginlib-0.9.0/doc/conf.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     2707 2018-07-17 02:26:58.000000 pluginlib-0.9.0/doc/error_handling.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)     4661 2020-05-02 19:07:31.000000 pluginlib-0.9.0/doc/faq.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)     3915 2020-04-28 13:48:21.000000 pluginlib-0.9.0/doc/index.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)       87 2018-07-30 14:56:06.000000 pluginlib-0.9.0/doc/spelling_wordlist.txt
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.224416 pluginlib-0.9.0/pluginlib/
--rw-rw-r--   0 avram     (1000) avram     (1000)     1006 2022-02-13 21:20:09.000000 pluginlib-0.9.0/pluginlib/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)    16845 2022-02-13 15:40:03.000000 pluginlib-0.9.0/pluginlib/_loader.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     8939 2022-02-13 13:52:50.000000 pluginlib-0.9.0/pluginlib/_objects.py
--rw-r--r--   0 avram     (1000) avram     (1000)    16590 2022-02-13 18:05:31.000000 pluginlib-0.9.0/pluginlib/_parent.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     6610 2022-02-13 15:32:15.000000 pluginlib-0.9.0/pluginlib/_util.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     1688 2022-02-13 13:25:39.000000 pluginlib-0.9.0/pluginlib/exceptions.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.225416 pluginlib-0.9.0/pluginlib.egg-info/
--rw-rw-r--   0 avram     (1000) avram     (1000)     9598 2022-02-13 21:36:48.000000 pluginlib-0.9.0/pluginlib.egg-info/PKG-INFO
--rw-rw-r--   0 avram     (1000) avram     (1000)     1375 2022-02-13 21:36:48.000000 pluginlib-0.9.0/pluginlib.egg-info/SOURCES.txt
--rw-rw-r--   0 avram     (1000) avram     (1000)        1 2022-02-13 21:36:48.000000 pluginlib-0.9.0/pluginlib.egg-info/dependency_links.txt
--rw-rw-r--   0 avram     (1000) avram     (1000)        1 2018-08-06 20:52:27.000000 pluginlib-0.9.0/pluginlib.egg-info/not-zip-safe
--rw-rw-r--   0 avram     (1000) avram     (1000)       11 2022-02-13 21:36:48.000000 pluginlib-0.9.0/pluginlib.egg-info/requires.txt
--rw-rw-r--   0 avram     (1000) avram     (1000)       10 2022-02-13 21:36:48.000000 pluginlib-0.9.0/pluginlib.egg-info/top_level.txt
--rw-rw-r--   0 avram     (1000) avram     (1000)      571 2022-02-13 21:36:48.230416 pluginlib-0.9.0/setup.cfg
--rw-rw-r--   0 avram     (1000) avram     (1000)     2164 2022-02-13 15:53:51.000000 pluginlib-0.9.0/setup.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     2508 2020-08-16 11:52:05.000000 pluginlib-0.9.0/setup_helpers.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.226416 pluginlib-0.9.0/tests/
--rw-rw-r--   0 avram     (1000) avram     (1000)     1743 2022-02-13 15:29:39.000000 pluginlib-0.9.0/tests/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     2588 2018-07-18 01:07:26.000000 pluginlib-0.9.0/tests/test_exceptions.py
--rw-rw-r--   0 avram     (1000) avram     (1000)    20686 2022-02-13 14:42:59.000000 pluginlib-0.9.0/tests/test_loader.py
--rw-rw-r--   0 avram     (1000) avram     (1000)    16119 2020-05-02 18:59:00.000000 pluginlib-0.9.0/tests/test_objects.py
--rw-rw-r--   0 avram     (1000) avram     (1000)    25910 2022-02-13 15:29:16.000000 pluginlib-0.9.0/tests/test_parent.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     7473 2022-02-13 15:23:29.000000 pluginlib-0.9.0/tests/test_util.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.226416 pluginlib-0.9.0/tests/testdata/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:03:46.000000 pluginlib-0.9.0/tests/testdata/__init__.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.226416 pluginlib-0.9.0/tests/testdata/bad/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-01 15:23:47.000000 pluginlib-0.9.0/tests/testdata/bad/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      408 2020-06-02 13:34:23.000000 pluginlib-0.9.0/tests/testdata/bad/syntax.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      533 2020-06-01 15:26:37.000000 pluginlib-0.9.0/tests/testdata/bad2.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.220416 pluginlib-0.9.0/tests/testdata/bare/
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.227416 pluginlib-0.9.0/tests/testdata/bare/engines/
--rw-rw-r--   0 avram     (1000) avram     (1000)      524 2020-06-02 05:00:57.000000 pluginlib-0.9.0/tests/testdata/bare/engines/electric.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.227416 pluginlib-0.9.0/tests/testdata/bare/hooks/
--rw-rw-r--   0 avram     (1000) avram     (1000)      553 2022-02-13 14:41:50.000000 pluginlib-0.9.0/tests/testdata/bare/hooks/fish.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      550 2020-06-02 05:04:18.000000 pluginlib-0.9.0/tests/testdata/bare/hooks/grappling.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.227416 pluginlib-0.9.0/tests/testdata/bare/package/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-02 04:46:13.000000 pluginlib-0.9.0/tests/testdata/bare/package/__init__.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.227416 pluginlib-0.9.0/tests/testdata/bare/package/parsers/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-02 04:46:24.000000 pluginlib-0.9.0/tests/testdata/bare/package/parsers/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      535 2020-06-02 05:02:36.000000 pluginlib-0.9.0/tests/testdata/bare/package/parsers/silly_walks.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.227416 pluginlib-0.9.0/tests/testdata/importer/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-15 02:39:55.000000 pluginlib-0.9.0/tests/testdata/importer/__init__.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.228416 pluginlib-0.9.0/tests/testdata/lib/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:04.000000 pluginlib-0.9.0/tests/testdata/lib/__init__.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.228416 pluginlib-0.9.0/tests/testdata/lib/engines/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-08 01:55:41.000000 pluginlib-0.9.0/tests/testdata/lib/engines/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      512 2020-06-02 05:03:03.000000 pluginlib-0.9.0/tests/testdata/lib/engines/steam.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.228416 pluginlib-0.9.0/tests/testdata/lib/hooks/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:38.000000 pluginlib-0.9.0/tests/testdata/lib/hooks/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      530 2020-06-02 05:03:14.000000 pluginlib-0.9.0/tests/testdata/lib/hooks/left.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      534 2020-06-02 05:03:22.000000 pluginlib-0.9.0/tests/testdata/lib/hooks/right.py
-drwxrwxr-x   0 avram     (1000) avram     (1000)        0 2022-02-13 21:36:48.229416 pluginlib-0.9.0/tests/testdata/lib/parsers/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:38.000000 pluginlib-0.9.0/tests/testdata/lib/parsers/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      669 2020-06-02 05:04:01.000000 pluginlib-0.9.0/tests/testdata/lib/parsers/json.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      503 2020-06-02 05:03:52.000000 pluginlib-0.9.0/tests/testdata/lib/parsers/xml.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      760 2018-07-09 01:05:42.000000 pluginlib-0.9.0/tests/testdata/parents.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/
+-rw-rw-r--   0 avram     (1000) avram     (1000)    16726 2017-10-10 15:55:09.000000 pluginlib-0.9.1/LICENSE
+-rw-rw-r--   0 avram     (1000) avram     (1000)       97 2022-02-13 15:53:51.000000 pluginlib-0.9.1/MANIFEST.in
+-rw-r--r--   0 avram     (1000) avram     (1000)     9642 2023-06-13 01:08:07.519497 pluginlib-0.9.1/PKG-INFO
+-rw-rw-r--   0 avram     (1000) avram     (1000)     8286 2022-12-30 13:57:46.000000 pluginlib-0.9.1/README.rst
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.517497 pluginlib-0.9.1/doc/
+-rw-rw-r--   0 avram     (1000) avram     (1000)     1575 2020-06-03 01:12:58.000000 pluginlib-0.9.1/doc/api.rst
+-rw-rw-r--   0 avram     (1000) avram     (1000)     8896 2018-08-28 12:21:53.000000 pluginlib-0.9.1/doc/concepts.rst
+-rw-rw-r--   0 avram     (1000) avram     (1000)     3648 2022-06-02 12:47:07.000000 pluginlib-0.9.1/doc/conf.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     2707 2018-07-17 02:26:58.000000 pluginlib-0.9.1/doc/error_handling.rst
+-rw-rw-r--   0 avram     (1000) avram     (1000)     4661 2020-05-02 19:07:31.000000 pluginlib-0.9.1/doc/faq.rst
+-rw-r--r--   0 avram     (1000) avram     (1000)     3915 2022-06-02 12:45:02.000000 pluginlib-0.9.1/doc/index.rst
+-rw-rw-r--   0 avram     (1000) avram     (1000)       87 2018-07-30 14:56:06.000000 pluginlib-0.9.1/doc/spelling_wordlist.txt
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/pluginlib/
+-rw-r--r--   0 avram     (1000) avram     (1000)     1006 2023-06-12 23:57:19.000000 pluginlib-0.9.1/pluginlib/__init__.py
+-rw-r--r--   0 avram     (1000) avram     (1000)    16942 2023-06-12 23:57:06.000000 pluginlib-0.9.1/pluginlib/_loader.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     8939 2023-06-12 23:44:40.000000 pluginlib-0.9.1/pluginlib/_objects.py
+-rw-r--r--   0 avram     (1000) avram     (1000)    16642 2023-06-12 23:44:42.000000 pluginlib-0.9.1/pluginlib/_parent.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     6520 2023-06-12 23:44:45.000000 pluginlib-0.9.1/pluginlib/_util.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     1688 2023-06-12 23:44:47.000000 pluginlib-0.9.1/pluginlib/exceptions.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/pluginlib.egg-info/
+-rw-rw-r--   0 avram     (1000) avram     (1000)     9642 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/PKG-INFO
+-rw-rw-r--   0 avram     (1000) avram     (1000)     1375 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 avram     (1000) avram     (1000)        1 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 avram     (1000) avram     (1000)        1 2018-08-06 20:52:27.000000 pluginlib-0.9.1/pluginlib.egg-info/not-zip-safe
+-rw-rw-r--   0 avram     (1000) avram     (1000)       11 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/requires.txt
+-rw-rw-r--   0 avram     (1000) avram     (1000)       10 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/top_level.txt
+-rw-rw-r--   0 avram     (1000) avram     (1000)      571 2023-06-13 01:08:07.520497 pluginlib-0.9.1/setup.cfg
+-rw-r--r--   0 avram     (1000) avram     (1000)     2215 2023-06-12 23:57:12.000000 pluginlib-0.9.1/setup.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     2508 2020-08-16 11:52:05.000000 pluginlib-0.9.1/setup_helpers.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/
+-rw-rw-r--   0 avram     (1000) avram     (1000)     1743 2023-06-12 23:45:31.000000 pluginlib-0.9.1/tests/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     2588 2023-06-12 23:45:33.000000 pluginlib-0.9.1/tests/test_exceptions.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)    20686 2023-06-12 23:45:35.000000 pluginlib-0.9.1/tests/test_loader.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)    16120 2023-06-12 23:45:37.000000 pluginlib-0.9.1/tests/test_objects.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)    25795 2023-06-12 23:45:39.000000 pluginlib-0.9.1/tests/test_parent.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     7473 2023-06-12 23:45:40.000000 pluginlib-0.9.1/tests/test_util.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/testdata/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:03:46.000000 pluginlib-0.9.1/tests/testdata/__init__.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/testdata/bad/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-01 15:23:47.000000 pluginlib-0.9.1/tests/testdata/bad/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      408 2020-06-02 13:34:23.000000 pluginlib-0.9.1/tests/testdata/bad/syntax.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      533 2020-06-01 15:26:37.000000 pluginlib-0.9.1/tests/testdata/bad2.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.516497 pluginlib-0.9.1/tests/testdata/bare/
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/testdata/bare/engines/
+-rw-rw-r--   0 avram     (1000) avram     (1000)      524 2020-06-02 05:00:57.000000 pluginlib-0.9.1/tests/testdata/bare/engines/electric.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/testdata/bare/hooks/
+-rw-rw-r--   0 avram     (1000) avram     (1000)      553 2022-02-13 14:41:50.000000 pluginlib-0.9.1/tests/testdata/bare/hooks/fish.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      550 2020-06-02 05:04:18.000000 pluginlib-0.9.1/tests/testdata/bare/hooks/grappling.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/bare/package/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-02 04:46:13.000000 pluginlib-0.9.1/tests/testdata/bare/package/__init__.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/bare/package/parsers/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-02 04:46:24.000000 pluginlib-0.9.1/tests/testdata/bare/package/parsers/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      535 2020-06-02 05:02:36.000000 pluginlib-0.9.1/tests/testdata/bare/package/parsers/silly_walks.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/importer/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-15 02:39:55.000000 pluginlib-0.9.1/tests/testdata/importer/__init__.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/lib/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:04.000000 pluginlib-0.9.1/tests/testdata/lib/__init__.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/lib/engines/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-08 01:55:41.000000 pluginlib-0.9.1/tests/testdata/lib/engines/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      512 2020-06-02 05:03:03.000000 pluginlib-0.9.1/tests/testdata/lib/engines/steam.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/lib/hooks/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:38.000000 pluginlib-0.9.1/tests/testdata/lib/hooks/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      530 2020-06-02 05:03:14.000000 pluginlib-0.9.1/tests/testdata/lib/hooks/left.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      534 2020-06-02 05:03:22.000000 pluginlib-0.9.1/tests/testdata/lib/hooks/right.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/lib/parsers/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:38.000000 pluginlib-0.9.1/tests/testdata/lib/parsers/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      669 2020-06-02 05:04:01.000000 pluginlib-0.9.1/tests/testdata/lib/parsers/json.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      503 2020-06-02 05:03:52.000000 pluginlib-0.9.1/tests/testdata/lib/parsers/xml.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      760 2018-07-09 01:05:42.000000 pluginlib-0.9.1/tests/testdata/parents.py
```

### Comparing `pluginlib-0.9.0/LICENSE` & `pluginlib-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/PKG-INFO` & `pluginlib-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pluginlib
-Version: 0.9.0
+Version: 0.9.1
 Summary: A framework for creating and importing plugins
 Home-page: https://github.com/Rockhopper-Technologies/pluginlib
 Author: Avram Lubkin
 Author-email: avylove@rockhopper.net
 License: MPLv2.0
 Keywords: plugin,plugins,pluginlib
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 .. start-badges
 
@@ -35,15 +35,15 @@
 | |pypi| |supported-versions| |supported-implementations|
 | |fedora| |EPEL|
 
 .. |docs| image:: https://img.shields.io/readthedocs/pluginlib.svg?style=plastic&logo=read-the-docs
     :target: https://pluginlib.readthedocs.org
     :alt: Documentation Status
 
-.. |gh_actions| image:: https://img.shields.io/github/workflow/status/Rockhopper-Technologies/pluginlib/Tests?event=push&logo=github-actions&style=plastic
+.. |gh_actions| image:: https://img.shields.io/github/actions/workflow/status/Rockhopper-Technologies/pluginlib/tests.yml?event=push&logo=github-actions&style=plastic
     :target: https://github.com/Rockhopper-Technologies/pluginlib/actions/workflows/tests.yml
     :alt: GitHub Actions Status
 
 .. |travis| image:: https://img.shields.io/travis/com/Rockhopper-Technologies/pluginlib.svg?style=plastic&logo=travis
     :target: https://travis-ci.com/Rockhopper-Technologies/pluginlib
     :alt: Travis-CI Build Status
 
@@ -242,9 +242,7 @@
 .. _accessed: http://pluginlib.readthedocs.io/en/stable/concepts.html#accessing-plugins
 .. _Abstract Methods: http://pluginlib.readthedocs.io/en/stable/concepts.html#abstract-methods
 .. _Conditional Loading: http://pluginlib.readthedocs.io/en/stable/concepts.html#conditional-loading
 .. _Plugin Groups: http://pluginlib.readthedocs.io/en/stable/concepts.html#plugin-groups
 
 .. _EPEL: https://fedoraproject.org/wiki/EPEL
 .. _configured: https://docs.fedoraproject.org/en-US/epel/#how_can_i_use_these_extra_packages
-
-
```

### Comparing `pluginlib-0.9.0/README.rst` & `pluginlib-0.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 | |pypi| |supported-versions| |supported-implementations|
 | |fedora| |EPEL|
 
 .. |docs| image:: https://img.shields.io/readthedocs/pluginlib.svg?style=plastic&logo=read-the-docs
     :target: https://pluginlib.readthedocs.org
     :alt: Documentation Status
 
-.. |gh_actions| image:: https://img.shields.io/github/workflow/status/Rockhopper-Technologies/pluginlib/Tests?event=push&logo=github-actions&style=plastic
+.. |gh_actions| image:: https://img.shields.io/github/actions/workflow/status/Rockhopper-Technologies/pluginlib/tests.yml?event=push&logo=github-actions&style=plastic
     :target: https://github.com/Rockhopper-Technologies/pluginlib/actions/workflows/tests.yml
     :alt: GitHub Actions Status
 
 .. |travis| image:: https://img.shields.io/travis/com/Rockhopper-Technologies/pluginlib.svg?style=plastic&logo=travis
     :target: https://travis-ci.com/Rockhopper-Technologies/pluginlib
     :alt: Travis-CI Build Status
```

### Comparing `pluginlib-0.9.0/doc/api.rst` & `pluginlib-0.9.1/doc/api.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/doc/concepts.rst` & `pluginlib-0.9.1/doc/concepts.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/doc/conf.py` & `pluginlib-0.9.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `pluginlib-0.9.0/doc/error_handling.rst` & `pluginlib-0.9.1/doc/error_handling.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/doc/faq.rst` & `pluginlib-0.9.1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/doc/index.rst` & `pluginlib-0.9.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/pluginlib/__init__.py` & `pluginlib-0.9.1/pluginlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 **Pluginlib Package**
 
 A framework for creating and importing plugins
 """
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 __all__ = ['abstractmethod', 'abstractproperty', 'abstractstaticmethod', 'abstractclassmethod',
            'abstractattribute', 'BlacklistEntry', 'EntryPointWarning', 'Parent', 'Plugin',
            'PluginlibError', 'PluginImportError', 'PluginLoader', 'PluginWarning']
 
 from abc import abstractmethod, abstractproperty
```

### Comparing `pluginlib-0.9.0/pluginlib/_loader.py` & `pluginlib-0.9.1/pluginlib/_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2023 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Pluginlib Loader Submodule**
@@ -19,15 +19,15 @@
 import warnings
 
 from pkg_resources import iter_entry_points, EntryPoint
 
 from pluginlib.exceptions import PluginImportError, EntryPointWarning
 from pluginlib._objects import BlacklistEntry
 from pluginlib._parent import get_plugins
-from pluginlib._util import BASESTRING, LOGGER, NoneType, PY2, PY34, raise_with_traceback
+from pluginlib._util import BASESTRING, LOGGER, NoneType, PY2, raise_with_traceback
 
 try:
     from collections.abc import Iterable
 except ImportError:   # pragma: no cover
     # For Python < 3.3
     from collections import Iterable  # pylint: disable=deprecated-class
 
@@ -110,15 +110,18 @@
     epoint = None
     if isinstance(name, EntryPoint):
         epoint = name
         name = epoint.module_name
 
     if path is None:
         try:
-            loader = pkgutil.get_loader(name)
+            if PY2:
+                loader = pkgutil.get_loader(name)  # pragma: no cover
+            else:
+                loader = getattr(importlib.util.find_spec(name), 'loader', None)
         except ImportError:
             pass
         else:
             if loader:
                 path = os.path.dirname(loader.get_filename(name))
 
     LOGGER.debug('Attempting to load module %s from %s', name, path)
@@ -185,16 +188,16 @@
             prefix = prefix_template % relpath.replace(os.sep, '.')
 
         # Walk root and import modules
         # pylint: disable=unused-variable
         for finder, name, is_pkg in pkgutil.walk_packages([root], prefix=prefix):
             LOGGER.debug('Attempting to load module %s from %s', name, finder.path)
             try:
-                # find_module() was deprecated in 3.4, but module_from_spec wasn't available
-                if PY34:  # pragma: no cover
+                # find_module() was deprecated in 3.4
+                if PY2:  # pragma: no cover
                     finder.find_module(name).load_module(name)
                 else:
                     spec = finder.find_spec(name)
                     module = importlib.util.module_from_spec(spec)
                     sys.modules[name] = module
                     spec.loader.exec_module(module)
```

### Comparing `pluginlib-0.9.0/pluginlib/_objects.py` & `pluginlib-0.9.1/pluginlib/_objects.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/pluginlib/_parent.py` & `pluginlib-0.9.1/pluginlib/_parent.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pluginlib._objects import GroupDict, TypeDict, PluginDict
 from pluginlib._util import (allow_bare_decorator, ClassProperty, DictWithDotNotation,
                              LOGGER, Undefined)
 
 try:
     from asyncio import iscoroutinefunction
 except ImportError:  # pragma: no cover
+    # pylint: disable=unnecessary-lambda-assignment
     iscoroutinefunction = lambda func: False  # noqa: E731
 
 
 DEFAULT = '_default'
 UNDEFINED = Undefined()
 
 isfunction = inspect.isfunction  # pylint: disable=invalid-name
```

### Comparing `pluginlib-0.9.0/pluginlib/_util.py` & `pluginlib-0.9.1/pluginlib/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from inspect import isclass
 import logging
 import operator as _operator
 import sys
 
 
 PY2 = sys.version_info[0] == 2
-PY34 = sys.version_info[:2] < (3, 5)
 
 
 # Setup logger
 LOGGER = logging.getLogger('pluginlib')
 LOGGER.addHandler(logging.NullHandler())
 
 OPERATORS = {'=': _operator.eq,
@@ -159,34 +158,34 @@
             self._cache.clear()
 
     def setdefault(self, key, default=None):
 
         try:
             return self[key]
         except KeyError:
-            self.__setitem__(key, default)
+            self[key] = default
             return default
 
     def pop(self, *args):
         try:
             value = super(CachingDict, self).pop(*args)
         except KeyError as e:
             raise e
-        else:
-            self._cache.clear()
-            return value
+
+        self._cache.clear()
+        return value
 
     def popitem(self):
         try:
             item = super(CachingDict, self).popitem()
         except KeyError as e:
             raise e
-        else:
-            self._cache.clear()
-            return item
+
+        self._cache.clear()
+        return item
 
 
 class DictWithDotNotation(dict):
     """
     Dictionary addressable by dot notation
     """
```

### Comparing `pluginlib-0.9.0/pluginlib/exceptions.py` & `pluginlib-0.9.1/pluginlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/pluginlib.egg-info/PKG-INFO` & `pluginlib-0.9.1/pluginlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pluginlib
-Version: 0.9.0
+Version: 0.9.1
 Summary: A framework for creating and importing plugins
 Home-page: https://github.com/Rockhopper-Technologies/pluginlib
 Author: Avram Lubkin
 Author-email: avylove@rockhopper.net
 License: MPLv2.0
 Keywords: plugin,plugins,pluginlib
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 .. start-badges
 
@@ -35,15 +35,15 @@
 | |pypi| |supported-versions| |supported-implementations|
 | |fedora| |EPEL|
 
 .. |docs| image:: https://img.shields.io/readthedocs/pluginlib.svg?style=plastic&logo=read-the-docs
     :target: https://pluginlib.readthedocs.org
     :alt: Documentation Status
 
-.. |gh_actions| image:: https://img.shields.io/github/workflow/status/Rockhopper-Technologies/pluginlib/Tests?event=push&logo=github-actions&style=plastic
+.. |gh_actions| image:: https://img.shields.io/github/actions/workflow/status/Rockhopper-Technologies/pluginlib/tests.yml?event=push&logo=github-actions&style=plastic
     :target: https://github.com/Rockhopper-Technologies/pluginlib/actions/workflows/tests.yml
     :alt: GitHub Actions Status
 
 .. |travis| image:: https://img.shields.io/travis/com/Rockhopper-Technologies/pluginlib.svg?style=plastic&logo=travis
     :target: https://travis-ci.com/Rockhopper-Technologies/pluginlib
     :alt: Travis-CI Build Status
 
@@ -242,9 +242,7 @@
 .. _accessed: http://pluginlib.readthedocs.io/en/stable/concepts.html#accessing-plugins
 .. _Abstract Methods: http://pluginlib.readthedocs.io/en/stable/concepts.html#abstract-methods
 .. _Conditional Loading: http://pluginlib.readthedocs.io/en/stable/concepts.html#conditional-loading
 .. _Plugin Groups: http://pluginlib.readthedocs.io/en/stable/concepts.html#plugin-groups
 
 .. _EPEL: https://fedoraproject.org/wiki/EPEL
 .. _configured: https://docs.fedoraproject.org/en-US/epel/#how_can_i_use_these_extra_packages
-
-
```

### Comparing `pluginlib-0.9.0/pluginlib.egg-info/SOURCES.txt` & `pluginlib-0.9.1/pluginlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/setup.cfg` & `pluginlib-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/setup.py` & `pluginlib-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,21 +41,22 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)',
         'Operating System :: POSIX',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: MacOS',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     keywords='plugin, plugins, pluginlib',
     test_loader="unittest:TestLoader"
 )
```

### Comparing `pluginlib-0.9.0/setup_helpers.py` & `pluginlib-0.9.1/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/__init__.py` & `pluginlib-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/test_exceptions.py` & `pluginlib-0.9.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/test_loader.py` & `pluginlib-0.9.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/test_objects.py` & `pluginlib-0.9.1/tests/test_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         self.assertEqual(self.tdict._filter(blacklist), self.expected)
         self.mock_plugin_json._filter.assert_called_with(blacklist, newest_only=False)
         self.mock_plugin_xml._filter.assert_called_with(blacklist, newest_only=False)
         mock_plugin_empty._filter.assert_called_with(blacklist, newest_only=False)
 
     def test_type_filter(self):
         """type_filter ignored in type dict"""
-        self.assertEqual(self.tdict._filter(type_filter=('engine')), self.expected)
+        self.assertEqual(self.tdict._filter(type_filter=('engine',)), self.expected)
 
     def test_name(self):
         """Get a specific name"""
         self.assertEqual(self.tdict._filter(name='json'), 'jsonplugin')
         self.mock_plugin_json._filter.assert_called_with(None, newest_only=False, name='json')
 
         self.assertIsNone(self.tdict._filter(name='pengion'))
```

### Comparing `pluginlib-0.9.0/tests/test_parent.py` & `pluginlib-0.9.1/tests/test_parent.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,14 @@
                        abstractclassmethod, abstractattribute)
 import pluginlib._parent as parent
 from pluginlib._util import PY2
 
 from tests import OUTPUT, TestCase, unittest
 
 
-NO_ASYNC = sys.version_info[:2] < (3, 5)
-
-
 # pylint: disable=protected-access, no-member
 
 
 # This should be imported from types, but it's broken in pypy
 # https://bitbucket.org/pypy/pypy/issues/2865
 class Placeholder(object):
     """Placeholder to get type"""
@@ -101,15 +98,15 @@
         If peers is True, another class is created with the same alias
         """
 
         @parent.Parent('test_parent')
         class Parent(object):
             """Parent"""
 
-            def hello(self):  # pylint: disable=no-self-use
+            def hello(self):
                 """Hello, world!"""
                 return 'world'
 
         if peers:
 
             class Child(Parent):
                 """Child"""
@@ -178,15 +175,15 @@
 
     def setUp(self):
 
         @parent.Parent('test_parent')
         class Parent(object):
             """Parent"""
 
-            def hello(self):  # pylint: disable=no-self-use
+            def hello(self):
                 """Hello, world!"""
                 return 'world'
 
         self.parent = Parent
         self.plugins = self.parent._get_plugins()
 
     def tearDown(self):
@@ -522,15 +519,15 @@
         self.missing(Parent, 'Does not contain required attribute')
         self.meth(Parent)
         self.static(Parent)
         self.klass(Parent)
         self.prop(Parent)
         self.attr(Parent)
 
-    @unittest.skipIf(NO_ASYNC, 'Requires Python 3.5+')
+    @unittest.skipIf(PY2, 'Requires Python 3.5+')
     def test_abstract_coroutine(self):
         """Attribute required in subclass"""
 
         @parent.Parent('test_parent')
         class Parent(object):
             """Parent with abstract coroutine"""
 
@@ -688,15 +685,15 @@
                 abstract = 'No one expects the abstract attribute'
 
         self.check_method(parent_class, error, Attr, e)
 
     def coroutine(self, parent_class, error=None):
         """Test abstract coroutine method"""
 
-        if NO_ASYNC:
+        if PY2:
             return
 
         with warnings.catch_warnings(record=True) as e:
 
             class_definition = textwrap.dedent('''\
             class Coroutine(parent_class):
                 """Only has coroutine method"""
```

### Comparing `pluginlib-0.9.0/tests/test_util.py` & `pluginlib-0.9.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/bad2.py` & `pluginlib-0.9.1/tests/testdata/bad2.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/bare/engines/electric.py` & `pluginlib-0.9.1/tests/testdata/bare/engines/electric.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/bare/hooks/fish.py` & `pluginlib-0.9.1/tests/testdata/bare/hooks/fish.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/bare/hooks/grappling.py` & `pluginlib-0.9.1/tests/testdata/bare/hooks/grappling.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/bare/package/parsers/silly_walks.py` & `pluginlib-0.9.1/tests/testdata/bare/package/parsers/silly_walks.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/lib/engines/steam.py` & `pluginlib-0.9.1/tests/testdata/lib/engines/steam.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/lib/hooks/left.py` & `pluginlib-0.9.1/tests/testdata/lib/hooks/left.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/lib/hooks/right.py` & `pluginlib-0.9.1/tests/testdata/lib/hooks/right.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/lib/parsers/json.py` & `pluginlib-0.9.1/tests/testdata/lib/parsers/json.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.0/tests/testdata/parents.py` & `pluginlib-0.9.1/tests/testdata/parents.py`

 * *Files identical despite different names*

