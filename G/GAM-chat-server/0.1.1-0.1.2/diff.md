# Comparing `tmp/GAM_chat_server-0.1.1.tar.gz` & `tmp/GAM_chat_server-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GAM_chat_server-0.1.1.tar", last modified: Tue Jun 13 17:12:55 2023, max compression
+gzip compressed data, was "GAM_chat_server-0.1.2.tar", last modified: Tue Jun 13 17:14:02 2023, max compression
```

## Comparing `GAM_chat_server-0.1.1.tar` & `GAM_chat_server-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 17:12:55.785249 GAM_chat_server-0.1.1/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 17:12:55.785249 GAM_chat_server-0.1.1/GAM_chat_server.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      140 2023-06-13 17:12:55.000000 GAM_chat_server-0.1.1/GAM_chat_server.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      202 2023-06-13 17:12:55.000000 GAM_chat_server-0.1.1/GAM_chat_server.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-13 17:12:55.000000 GAM_chat_server-0.1.1/GAM_chat_server.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-13 17:12:55.000000 GAM_chat_server-0.1.1/GAM_chat_server.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-13 17:12:55.000000 GAM_chat_server-0.1.1/GAM_chat_server.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      140 2023-06-13 17:12:55.785249 GAM_chat_server-0.1.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-13 17:12:55.785249 GAM_chat_server-0.1.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      294 2023-06-13 17:10:59.000000 GAM_chat_server-0.1.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 17:14:02.341141 GAM_chat_server-0.1.2/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 17:14:02.337140 GAM_chat_server-0.1.2/GAM_chat_server.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      154 2023-06-13 17:14:02.000000 GAM_chat_server-0.1.2/GAM_chat_server.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      202 2023-06-13 17:14:02.000000 GAM_chat_server-0.1.2/GAM_chat_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-13 17:14:02.000000 GAM_chat_server-0.1.2/GAM_chat_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-13 17:14:02.000000 GAM_chat_server-0.1.2/GAM_chat_server.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-13 17:14:02.000000 GAM_chat_server-0.1.2/GAM_chat_server.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      154 2023-06-13 17:14:02.337140 GAM_chat_server-0.1.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-13 17:14:02.341141 GAM_chat_server-0.1.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      308 2023-06-13 17:13:59.000000 GAM_chat_server-0.1.2/setup.py
```

