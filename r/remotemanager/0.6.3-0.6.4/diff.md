# Comparing `tmp/remotemanager-0.6.3.tar.gz` & `tmp/remotemanager-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.6.3.tar", last modified: Mon Jun 12 10:02:48 2023, max compression
+gzip compressed data, was "remotemanager-0.6.4.tar", last modified: Tue Jun 13 14:19:40 2023, max compression
```

## Comparing `remotemanager-0.6.3.tar` & `remotemanager-0.6.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.095340 remotemanager-0.6.3/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-12 10:02:48.095340 remotemanager-0.6.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.6.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-06 06:58:31.000000 remotemanager-0.6.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.087339 remotemanager-0.6.3/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-06 06:58:31.000000 remotemanager-0.6.3/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15718 2023-06-08 13:33:35.000000 remotemanager-0.6.3/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12674 2023-05-31 07:19:00.000000 remotemanager-0.6.3/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.6.3/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.6.3/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.6.3/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.6.3/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    24882 2023-06-08 11:36:38.000000 remotemanager-0.6.3/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49754 2023-06-12 08:57:29.000000 remotemanager-0.6.3/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    22474 2023-06-12 08:57:29.000000 remotemanager-0.6.3/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.6.3/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-25 09:38:01.000000 remotemanager-0.6.3/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4325 2023-06-08 11:36:38.000000 remotemanager-0.6.3/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.6.3/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.6.3/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.6.3/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.6.3/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.6.3/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.095340 remotemanager-0.6.3/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.6.3/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.6.3/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.095340 remotemanager-0.6.3/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.6.3/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.6.3/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9262 2023-06-02 09:40:16.000000 remotemanager-0.6.3/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.095340 remotemanager-0.6.3/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.087339 remotemanager-0.6.3/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 10:02:48.095340 remotemanager-0.6.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.618359 remotemanager-0.6.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-13 14:19:40.618359 remotemanager-0.6.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.6.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-12 10:37:37.000000 remotemanager-0.6.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.610359 remotemanager-0.6.4/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-12 10:37:37.000000 remotemanager-0.6.4/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.610359 remotemanager-0.6.4/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15718 2023-06-08 13:33:35.000000 remotemanager-0.6.4/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.610359 remotemanager-0.6.4/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12730 2023-06-13 13:42:38.000000 remotemanager-0.6.4/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.6.4/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.6.4/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.6.4/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.6.4/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    24882 2023-06-08 11:36:38.000000 remotemanager-0.6.4/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49754 2023-06-12 08:57:29.000000 remotemanager-0.6.4/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    22474 2023-06-12 08:57:29.000000 remotemanager-0.6.4/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.6.4/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-25 09:38:01.000000 remotemanager-0.6.4/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4325 2023-06-08 11:36:38.000000 remotemanager-0.6.4/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.6.4/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.6.4/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.6.4/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.6.4/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.6.4/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.6.4/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.6.4/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.618359 remotemanager-0.6.4/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.6.4/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.6.4/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9262 2023-06-02 09:40:16.000000 remotemanager-0.6.4/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.618359 remotemanager-0.6.4/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.610359 remotemanager-0.6.4/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 14:19:40.618359 remotemanager-0.6.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.6.4/setup.py
```

### Comparing `remotemanager-0.6.3/LICENSE` & `remotemanager-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/PKG-INFO` & `remotemanager-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.3
+Version: 0.6.4
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.3/README.md` & `remotemanager-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/pyproject.toml` & `remotemanager-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.6.3"
+current_version = "0.6.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.6.3/remotemanager/connection/cmd.py` & `remotemanager-0.6.4/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/connection/computers/base.py` & `remotemanager-0.6.4/remotemanager/connection/computers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,25 +251,25 @@
             spec["resource_parser"] = self._parser
         else:
             spec["resource_parser"] = Function(self.parser)
 
         return spec
 
     @classmethod
-    def from_yaml(cls, filepath: str):
+    def from_yaml(cls, filepath: str, **url_args):
         if isinstance(filepath, str):
             with open(filepath, "r") as o:
                 data = yaml.safe_load(o)
         else:
             data = yaml.safe_load(filepath)
 
         # convert the parser back into a function
         data["resource_parser"] = Function.unpack(data["resource_parser"])
 
-        return cls.from_dict(data)
+        return cls.from_dict(data, **url_args)
 
     def to_yaml(self, filepath):
         data = self.serialise(self.to_dict())
 
         if isinstance(filepath, str):
             with open(filepath, "w+") as o:
                 yaml.dump(data, o)
@@ -278,14 +278,15 @@
 
     @classmethod
     def from_repo(
         cls,
         name: str,
         branch: str = "main",
         repo: str = "https://gitlab.com/l_sim/remotemanager-computers/",
+        **url_args,
     ):
         """
         Attempt to access the remote-computers repo, and pull the computer with name
         `name`
 
         Args:
             name (str):
@@ -315,15 +316,15 @@
         filename = ensure_filetype(name, "yaml").lower()
         url = f"{repo}-/raw/{branch}/storage/{filename}"
 
         print(f"polling url {url}")
 
         download_file(url, filename)
 
-        return cls.from_yaml(filename)
+        return cls.from_yaml(filename, **url_args)
 
     @property
     def parser(self):
         if not isinstance(self._parser, Function):
             self._parser = Function(self._parser)
         return self._parser.object
```

### Comparing `remotemanager-0.6.3/remotemanager/connection/computers/example.py` & `remotemanager-0.6.4/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/connection/computers/options.py` & `remotemanager-0.6.4/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/connection/computers/parsers.py` & `remotemanager-0.6.4/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/connection/testing_object.py` & `remotemanager-0.6.4/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/connection/url.py` & `remotemanager-0.6.4/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/dataset/dataset.py` & `remotemanager-0.6.4/remotemanager/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/dataset/dependency.py` & `remotemanager-0.6.4/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/dataset/runner.py` & `remotemanager-0.6.4/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/jupyter/magic.py` & `remotemanager-0.6.4/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/logging/__init__.py` & `remotemanager-0.6.4/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/logging/log.py` & `remotemanager-0.6.4/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/logging/utils.py` & `remotemanager-0.6.4/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/logging/verbosity.py` & `remotemanager-0.6.4/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/serialisation/serial.py` & `remotemanager-0.6.4/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.6.4/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.6.4/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/storage/database.py` & `remotemanager-0.6.4/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/storage/function.py` & `remotemanager-0.6.4/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/storage/remotefunction.py` & `remotemanager-0.6.4/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/storage/sendablemixin.py` & `remotemanager-0.6.4/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/storage/trackedfile.py` & `remotemanager-0.6.4/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/transport/cp.py` & `remotemanager-0.6.4/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/transport/rsync.py` & `remotemanager-0.6.4/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/transport/scp.py` & `remotemanager-0.6.4/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/transport/transport.py` & `remotemanager-0.6.4/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/utils/__init__.py` & `remotemanager-0.6.4/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/utils/flags.py` & `remotemanager-0.6.4/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager/utils/version.py` & `remotemanager-0.6.4/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.3/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.6.4/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.3
+Version: 0.6.4
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.3/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.6.4/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

