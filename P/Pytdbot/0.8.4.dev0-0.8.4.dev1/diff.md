# Comparing `tmp/Pytdbot-0.8.4.dev0.tar.gz` & `tmp/Pytdbot-0.8.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytdbot-0.8.4.dev0.tar", last modified: Tue May  2 05:33:50 2023, max compression
+gzip compressed data, was "Pytdbot-0.8.4.dev1.tar", last modified: Tue Jun 13 14:39:33 2023, max compression
```

## Comparing `Pytdbot-0.8.4.dev0.tar` & `Pytdbot-0.8.4.dev1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.580613 Pytdbot-0.8.4.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-02 05:33:50.580613 Pytdbot-0.8.4.dev0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.572613 Pytdbot-0.8.4.dev0/Pytdbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-02 05:33:50.000000 Pytdbot-0.8.4.dev0/Pytdbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-02 05:33:50.000000 Pytdbot-0.8.4.dev0/Pytdbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:33:50.000000 Pytdbot-0.8.4.dev0/Pytdbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 05:33:50.000000 Pytdbot-0.8.4.dev0/Pytdbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 05:33:50.000000 Pytdbot-0.8.4.dev0/Pytdbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.572613 Pytdbot-0.8.4.dev0/pytdbot/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44156 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.572613 Pytdbot-0.8.4.dev0/pytdbot/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/generate_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.572613 Pytdbot-0.8.4.dev0/pytdbot/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/handlers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   146663 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/handlers/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.576613 Pytdbot-0.8.4.dev0/pytdbot/methods/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57753 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/methods/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)   444864 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/methods/tdlibfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)  1248427 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/td_api.json
--rw-r--r--   0 runner    (1001) docker     (123)   585705 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/td_api.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.576613 Pytdbot-0.8.4.dev0/pytdbot/tdjson/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/tdjson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/tdjson/tdjson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.576613 Pytdbot-0.8.4.dev0/pytdbot/types/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.576613 Pytdbot-0.8.4.dev0/pytdbot/types/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/buttons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/buttons/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/buttons/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/buttons/inline_keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/buttons/remove_keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/buttons/show_keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.576613 Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_file_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_file_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.576613 Pytdbot-0.8.4.dev0/pytdbot/types/logstream/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/logstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/logstream/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/logstream/log_stream_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/logstream/log_stream_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/logstream/log_stream_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.576613 Pytdbot-0.8.4.dev0/pytdbot/types/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.576613 Pytdbot-0.8.4.dev0/pytdbot/types/result/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/result/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.580613 Pytdbot-0.8.4.dev0/pytdbot/types/update/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/update/chatActions.py
--rw-r--r--   0 runner    (1001) docker     (123)    60423 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/types/update/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:33:50.580613 Pytdbot-0.8.4.dev0/pytdbot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/pytdbot/utils/text_format.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:33:50.580613 Pytdbot-0.8.4.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-02 05:33:49.000000 Pytdbot-0.8.4.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.500946 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42708 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/generate_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/handlers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146663 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/handlers/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57920 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/methods/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   444864 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/methods/tdlibfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1248427 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/td_api.json
+-rw-r--r--   0 runner    (1001) docker     (123)   585705 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/td_api.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/tdjson/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/tdjson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/tdjson/tdjson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/inline_keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/remove_keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/show_keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/log_stream_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/log_stream_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/log_stream_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/result/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/result/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/update/chatActions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60488 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/update/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/utils/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/setup.py
```

### Comparing `Pytdbot-0.8.4.dev0/LICENSE` & `Pytdbot-0.8.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/PKG-INFO` & `Pytdbot-0.8.4.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytdbot
-Version: 0.8.4.dev0
+Version: 0.8.4.dev1
 Summary: Easy-to-use asynchronous TDLib wrapper for Python.
 Home-page: https://github.com/pytdbot/client
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/pytdbot/client
 Project-URL: Tracker, https://github.com/pytdbot/client/issues
@@ -28,17 +28,17 @@
 
 ### Requirements
 
 - Python 3.9+
 - Telegram [API key](https://my.telegram.org/apps)
 - [tdjson](https://github.com/tdlib/td#building)
 - [deepdiff](https://github.com/seperman/deepdiff)
-- [ujson](https://github.com/ultrajson/ultrajson)
 
 ### Installation
+> For better performance, it's recommended to install [orjson](https://github.com/ijl/orjson#install) or [ujson](https://github.com/ultrajson/ultrajson#ultrajson).
 
 ```bash
 pip install pytdbot
 ```
 From github (dev version)
 ```bash
 pip install git+https://github.com/pytdbot/client.git
```

### Comparing `Pytdbot-0.8.4.dev0/Pytdbot.egg-info/PKG-INFO` & `Pytdbot-0.8.4.dev1/Pytdbot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytdbot
-Version: 0.8.4.dev0
+Version: 0.8.4.dev1
 Summary: Easy-to-use asynchronous TDLib wrapper for Python.
 Home-page: https://github.com/pytdbot/client
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/pytdbot/client
 Project-URL: Tracker, https://github.com/pytdbot/client/issues
@@ -28,17 +28,17 @@
 
 ### Requirements
 
 - Python 3.9+
 - Telegram [API key](https://my.telegram.org/apps)
 - [tdjson](https://github.com/tdlib/td#building)
 - [deepdiff](https://github.com/seperman/deepdiff)
-- [ujson](https://github.com/ultrajson/ultrajson)
 
 ### Installation
+> For better performance, it's recommended to install [orjson](https://github.com/ijl/orjson#install) or [ujson](https://github.com/ultrajson/ultrajson#ultrajson).
 
 ```bash
 pip install pytdbot
 ```
 From github (dev version)
 ```bash
 pip install git+https://github.com/pytdbot/client.git
```

### Comparing `Pytdbot-0.8.4.dev0/Pytdbot.egg-info/SOURCES.txt` & `Pytdbot-0.8.4.dev1/Pytdbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/README.md` & `Pytdbot-0.8.4.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 ### Requirements
 
 - Python 3.9+
 - Telegram [API key](https://my.telegram.org/apps)
 - [tdjson](https://github.com/tdlib/td#building)
 - [deepdiff](https://github.com/seperman/deepdiff)
-- [ujson](https://github.com/ultrajson/ultrajson)
 
 ### Installation
+> For better performance, it's recommended to install [orjson](https://github.com/ijl/orjson#install) or [ujson](https://github.com/ultrajson/ultrajson#ultrajson).
 
 ```bash
 pip install pytdbot
 ```
 From github (dev version)
 ```bash
 pip install git+https://github.com/pytdbot/client.git
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/client.py` & `Pytdbot-0.8.4.dev1/pytdbot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from typing import Callable, Union
 from logging import getLogger, DEBUG
 from base64 import b64encode
 from deepdiff import DeepDiff
 from concurrent.futures import ThreadPoolExecutor
 from threading import current_thread, main_thread
-from ujson import dumps
+from json import dumps
 
 from .tdjson import TdJson
 from .handlers import Decorators, Handler
 from .methods import Methods
 from .types import Plugins, Result, LogStream, Update
 from .filters import Filter
 from .exception import StopHandlers, AuthorizationError
@@ -212,15 +212,14 @@
         """Start pytdbot client
 
         Args:
             login (``bool``, *optional*):
                 Login after start. Defaults to ``True``
         """
         if not self.is_running:
-
             logger.info("Starting pytdbot client...")
 
             self._workers_tasks = [
                 self.loop.create_task(self._update_worker(x + 1))
                 for x in range(self.workers)
             ]
 
@@ -247,22 +246,22 @@
                 return
 
         if not self.is_running:
             return
 
         self.me = await self.getMe()
         if self.me.is_error:
-            logger.error("Get me error: {}".format(self.me["message"]))
+            logger.error(f"Get me error: {self.me['message']}")
 
         self.me = self.me.result
         self.is_authenticated = True
         logger.info(
             "Logged in as {} {}".format(
                 self.me["first_name"],
-                self.me["id"].__str__()
+                str(self.me["id"])
                 if "usernames" not in self.me
                 else "@" + self.me["usernames"]["editable_username"],
             )
         )
 
     def add_handler(
         self,
@@ -356,68 +355,64 @@
 
         result = Result(request)
         self._results[result.id] = result
 
         if (
             logger.root.level >= DEBUG
         ):  # dumping all requests may create performance issues
-            logger.debug("Sending: {}".format(dumps(result.request, indent=4)))
+            logger.debug(f"Sending: {dumps(result.request, indent=4)}")
 
         self.__send(result.request)
         await result
 
         if result.is_error:
             if result["code"] == 429:
                 retry_after = self.get_retry_after_time(result["message"])
 
                 if retry_after <= self.sleep_threshold:
                     result.reset()
 
                     logger.error(
-                        "Sleeping for {}s (Caused by {})".format(
-                            retry_after, result.request["@type"]
-                        )
+                        f"Sleeping for {retry_after}s (Caused by {result.request['@type']})"
                     )
 
                     await asyncio.sleep(retry_after)
                     self._results[result.id] = result
                     self.__send(result.request)
                     await result
             elif not self.use_message_database and (
                 result["code"] == 400
                 and result["message"] == "Chat not found"
                 and "chat_id" in result.request
             ):
                 chat_id = result.request["chat_id"]
 
-                logger.debug("Attempt to load chat {}".format(chat_id))
+                logger.debug(f"Attempt to load chat {chat_id}")
 
                 load_chat = await self.getChat(chat_id)
 
                 if not load_chat.is_error:
-                    logger.debug("Chat {} is loaded".format(chat_id))
+                    logger.debug(f"Chat {chat_id} is loaded")
 
-                    message_id = 0
-                    if "reply_to_message_id" in result.request:
-                        message_id = result.request["reply_to_message_id"]
-                    elif "message_id" in result.request:
-                        message_id = result.request["message_id"]
+                    message_id = result.request.get(
+                        "reply_to_message_id", 0
+                    ) or result.request.get("message_id", 0)
 
                     # If there is a message_id then
                     # we need to load it to avoid MESSAGE_NOT_FOUND
                     if message_id > 0:
                         await self.getMessage(chat_id, message_id)
 
                     # repeat the first request
                     result.reset()
                     self._results[result.id] = result
                     self.__send(result.request)
                     await result
                 else:
-                    logger.error("Couldn't load chat {}".format(chat_id))
+                    logger.error(f"Couldn't load chat {chat_id}")
 
         return result
 
     async def call_method(self, method: str, **kwargs) -> Result:
         """Call a method. with keyword arguments (``kwargs``) support
 
         Example:
@@ -558,43 +553,37 @@
         count = 0
         handlers = 0
         for path in sorted(Path(self.plugins.folder).rglob("*.py")):
             module_path = ".".join(path.parent.parts + (path.stem,))
             try:
                 module = import_module(module_path)
             except Exception:
-                logger.exception("Failed to load plugin {}".format(module_path))
+                logger.exception(f"Failed to load plugin {module_path}")
             else:
-                logger.debug("Plugin {} loaded".format(module_path))
+                logger.debug(f"Plugin {module_path} loaded")
                 for name in dir(module):
                     obj = getattr(module, name)
                     if hasattr(obj, "_handler") and isinstance(obj._handler, Handler):
                         if asyncio.iscoroutinefunction(obj._handler.func):
                             self.add_handler(
                                 obj._handler.update_type,
                                 obj._handler.func,
                                 obj._handler.filter,
                                 obj._handler.position,
                             )
                             logger.debug(
-                                "Handler {} added from {}".format(
-                                    obj._handler.func,
-                                    module_path,
-                                )
+                                f"Handler {obj._handler.func} added from {module_path}"
                             )
                             handlers += 1
                         else:
                             logger.warn(
-                                "Handler {} is not an async function from module {}".format(
-                                    obj._handler.func,
-                                    module_path,
-                                )
+                                f"Handler {obj._handler.func} is not an async function from module {module_path}"
                             )
                 count += 1
-        logger.info("From {} plugins got {} handlers".format(count, handlers))
+        logger.info(f"From {count} plugins got {handlers} handlers")
 
     def is_coro_filter(self, func: Callable) -> bool:
         if func in self.__cache["is_coro_filter"]:
             return self.__cache["is_coro_filter"][func]
         else:
             is_coro = asyncio.iscoroutinefunction(func)
             self.__cache["is_coro_filter"][func] = is_coro
@@ -617,31 +606,26 @@
             self.is_running = False
 
     def _process_update(self, update):
         if "@client_id" in update:
             del update["@client_id"]
 
         if "@type" not in update:
-            logger.error("Unexpected update received: {}".format(update))
+            logger.error(f"Unexpected update received: {update}")
             return
         elif "@extra" in update:
             if (
                 logger.root.level >= DEBUG
             ):  # dumping all results may create performance issues
-                logger.debug("Recieved: {}".format(dumps(update, indent=4)))
+                logger.debug(f"Received: {dumps(update, indent=4)}")
             if update["@extra"]["id"] in self._results:
                 result: Result = self._results.pop(update["@extra"]["id"])
                 result.set_result(update)
             elif update["@type"] == "error" and "option" in update["@extra"]:
-                logger.error(
-                    "{}: {}".format(
-                        update["@extra"]["option"],
-                        update["message"],
-                    )
-                )
+                logger.error(f"{update['@extra']['option']}: {update['message']}")
         else:
             if update["@type"] == "updateAuthorizationState":
                 self.loop.create_task(self.__handle_authorization_state(update))
             elif update["@type"] == "updateMessageSendSucceeded":
                 self.loop.create_task(self.__handle_update_message_succeeded(update))
             elif update["@type"] == "updateMessageSendFailed":
                 self.loop.create_task(self.__handle_update_message_failed(update))
@@ -666,15 +650,15 @@
                     elif not filter_func(self, update):
                         continue
 
                 await initializer.func(self, update)
             except StopHandlers as e:
                 raise e
             except Exception:
-                logger.exception("Initializer {} failed".format(initializer))
+                logger.exception(f"Initializer {initializer} failed")
 
     async def __run_handlers(self, update):
         update_type = update["@type"]
         for handler in self._handlers[update_type]:
             try:
                 if handler.filter is not None:
                     filter_func = handler.filter.func
@@ -684,15 +668,15 @@
                     elif not filter_func(self, update):
                         continue
 
                 await handler.func(self, update)
             except StopHandlers as e:
                 raise e
             except Exception:
-                logger.exception("Exception in {}".format(handler))
+                logger.exception(f"Exception in {handler}")
 
     async def __run_finalizers(self, update):
         for finalizer in self._handlers["finalizer"]:
             try:
                 if finalizer.filter is not None:
                     filter_func = finalizer.filter.func
 
@@ -702,33 +686,32 @@
                     elif not filter_func(self, update):
                         continue
 
                 await finalizer.func(self, update)
             except StopHandlers as e:
                 raise e
             except Exception:
-                logger.exception("Finalizer {} failed".format(finalizer))
+                logger.exception(f"Finalizer {finalizer} failed")
 
     async def _update_worker(self, worker_id: int):
         self.is_running = True
         while self.is_running:
             try:
                 update = await self.queue.get()
                 if "@type" not in update:
                     continue
 
                 if (
                     logger.root.level >= DEBUG
                 ):  # dumping all updates can create performance issues
                     logger.debug(
-                        "w{}: Received: {}".format(worker_id, dumps(update, indent=4)),
+                        f"w{worker_id}: Received: {dumps(update, indent=4)}",
                     )
 
                 if update["@type"] in self._handlers:
-
                     update = self.update_class(self, update)
                     if (
                         update["@type"] == "updateNewMessage"
                         and update["message"]["is_outgoing"]
                         and "sending_state" in update["message"]
                     ):
                         continue
@@ -802,26 +785,24 @@
                 {
                     "@type": "setOption",
                     "name": k,
                     "value": data,
                     "@extra": {"option": k, "value": v, "id": ""},
                 }
             )
-            logger.debug("Option {} sent with value {}".format(k, str(v)))
+            logger.debug(f"Option {k} sent with value {v}")
 
     async def __handle_authorization_state(self, update):
         if update["@type"] == "updateAuthorizationState":
             old_authorization_state = self.authorization_state
             self.__authorization_state = update["authorization_state"]["@type"]
             self.__authorization = update["authorization_state"]
 
             logger.info(
-                "Authorization state changed to {}".format(
-                    self.authorization_state.removeprefix("authorizationState"),
-                )
+                f"Authorization state changed to {self.authorization_state.removeprefix('authorizationState')}"
             )
 
             if self.__login:
                 if self.authorization_state == "authorizationStateWaitTdlibParameters":
                     await self._set_options()
                     await self.set_td_paramaters()
                 elif self.authorization_state == "authorizationStateWaitPhoneNumber":
@@ -846,88 +827,75 @@
                 ):
                     self.__stop_client()
 
     async def __handle_connection_state(self, update):
         if update["@type"] == "updateConnectionState":
             self.connection_state: str = update["state"]["@type"]
             logger.info(
-                "Connection state changed to {}".format(
-                    self.connection_state.removeprefix("connectionState"),
-                )
+                f"Connection state changed to {self.connection_state.removeprefix('connectionState')}"
             )
 
     async def __handle_update_message_succeeded(self, update):
-        m_id = (
-            update["old_message_id"].__str__() + update["message"]["chat_id"].__str__()
-        )
+        m_id = str(update["old_message_id"]) + str(update["message"]["chat_id"])
 
         if m_id in self._results:
             result: Result = self._results.pop(m_id)
             result.set_result(update["message"])
 
     async def __handle_update_message_failed(self, update):
-        m_id = (
-            update["old_message_id"].__str__() + update["message"]["chat_id"].__str__()
-        )
+        m_id = str(update["old_message_id"]) + str(update["message"]["chat_id"])
 
         if m_id in self._results:
             if update["error_code"] == 429:
                 retry_after = update["message"]["sending_state"]["retry_after"]
 
                 if retry_after <= self.sleep_threshold:
                     result: Result = self._results.pop(m_id)
 
                     logger.error(
-                        "Sleeping for {}s (Caused by {})".format(
-                            int(retry_after), result.request["@type"]
-                        )
+                        f"Sleeping for {retry_after}s (Caused by {result.request['@type']})"
                     )
 
                     await asyncio.sleep(retry_after)
                     res = await self.invoke(result.request)
 
                     self._results[
-                        res.result["id"].__str__()
-                        + update["message"]["chat_id"].__str__()
+                        str(res.result["id"]) + str(update["message"]["chat_id"])
                     ] = result
             else:
                 result: Result = self._results.pop(m_id)
                 result.set_result(
                     {
                         "@type": "error",
                         "code": update["error_code"],
                         "message": update["error_message"],
                     }
                 )
 
     async def __handle_update_option(self, update):
-
         if update["value"]["@type"] == "optionValueBoolean":
             self.options[update["name"]] = bool(update["value"]["value"])
         elif update["value"]["@type"] == "optionValueEmpty":
             self.options[update["name"]] = None
         elif update["value"]["@type"] == "optionValueInteger":
             self.options[update["name"]] = int(update["value"]["value"])
         else:
             self.options[update["name"]] = update["value"]["value"]
 
         if self.is_authenticated:
             logger.info(
-                "Option {} changed to {}".format(
-                    update["name"],
-                    self.options[update["name"]],
-                )
+                f"Option {update['name']} changed to {self.options[update['name']]}"
             )
 
     async def __handle_update_user(self, update):
         if self.is_authenticated and update["user"]["id"] == self.me["id"]:
             logger.info(
                 "Updating {} ({}) info".format(
                     self.me["first_name"],
-                    self.me["id"].__str__()
+                    str(self.me["id"])
                     if "usernames" not in self.me
                     else "@" + self.me["usernames"]["editable_username"],
                 )
             )
             try:
                 deepdiff(self.me, update["user"])
             except Exception:
@@ -939,17 +907,15 @@
             return
 
         if not isinstance(self.__token, str):
             while self.is_running:
                 user_input = await self.__ainput("Enter a phone number or bot token: ")
 
                 if user_input:
-                    y_n = await self.__ainput(
-                        'Is "{}" correct? (y/n): '.format(user_input),
-                    )
+                    y_n = await self.__ainput(f'Is "{user_input}" correct? (y/n): ')
 
                     if y_n == "" or y_n.lower() in ["y", "yes"]:
                         if ":" in user_input:
                             res = await self.checkAuthenticationBotToken(user_input)
                         else:
                             res = await self.setAuthenticationPhoneNumber(user_input)
 
@@ -1013,15 +979,15 @@
         elif code_type == "authenticationCodeTypeMissedCall":
             code_type = "phone missed call"
         elif code_type == "authenticationCodeTypeFragment":
             code_type = "fragment.com SMS"
 
         while self.is_running:
             code = await self.__ainput(
-                "Enter the login code received via {}: ".format(code_type),
+                f"Enter the login code received via {code_type}: "
             )
 
             res = await self.checkAuthenticationCode(code=code)
             if res.is_error:
                 print(res["message"])
             else:
                 break
@@ -1041,19 +1007,15 @@
                 break
 
     async def __handle_authorization_state_wait_password(self):
         if self.authorization_state != "authorizationStateWaitPassword":
             return
 
         if self.__authorization["password_hint"]:
-            print(
-                "Your 2FA password hint is: {}".format(
-                    self.__authorization["password_hint"]
-                )
-            )
+            print(f"Your 2FA password hint is: {self.__authorization['password_hint']}")
 
         while self.is_running:
             password = await self.loop.run_in_executor(
                 self._executor,
                 getpass,
                 "Enter your 2FA password {}: ".format(
                     "(empty to recover)"
@@ -1072,19 +1034,15 @@
                         res = await self.requestAuthenticationPasswordRecovery()
 
                         if res.is_error:
                             raise AuthorizationError(res["message"])
                         else:
                             while True:
                                 recovery_code = await self.__ainput(
-                                    "Enter your recovery code sent to {}: ".format(
-                                        self.__authorization[
-                                            "recovery_email_address_pattern"
-                                        ]
-                                    ),
+                                    f"Enter your recovery code sent to {self.__authorization['recovery_email_address_pattern']}: "
                                 )
 
                                 res = (
                                     await self.checkAuthenticationPasswordRecoveryCode(
                                         recovery_code
                                     )
                                 )
@@ -1144,34 +1102,28 @@
             except NotImplementedError:  # Windows dosen't support add_signal_handler
                 pass
 
     def __ainput(self, prompt: str):
         return self.loop.run_in_executor(self._executor, input, prompt)
 
     def _print_welcome(self):
+        print(f"Welcome to Pytdbot (v{pytdbot.__version__}). {pytdbot.__copyright__}")
         print(
-            "Welcome to Pytdbot (v{}). {}".format(
-                pytdbot.__version__, pytdbot.__copyright__
-            )
-        )
-        print(
-            "Pytdbot is free software and comes with ABSOLUTELY NO WARRANTY. Licensed under the terms of {}.\n\n".format(
-                pytdbot.__license__
-            )
+            f"Pytdbot is free software and comes with ABSOLUTELY NO WARRANTY. Licensed under the terms of {pytdbot.__license__}.\n\n"
         )
 
 
 def deepdiff(d1, d2):
     if not isinstance(d1, dict) or not isinstance(d2, dict):
         return d1 == d2
 
     deep = DeepDiff(d1, d2, ignore_order=True, view="tree")
 
     for parent in deep.keys():
         for diff in deep[parent]:
             difflist = diff.path(output_format="list")
-            key = ".".join(v.__str__() for v in difflist)
+            key = ".".join(str(v) for v in difflist)
 
             if parent in ["dictionary_item_added", "values_changed"]:
                 logger.info(f"{key} changed to {diff.t2}")
             elif parent == "dictionary_item_removed":
                 logger.info(f"{key} removed")
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/filters.py` & `Pytdbot-0.8.4.dev1/pytdbot/filters.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/generate_files.py` & `Pytdbot-0.8.4.dev1/pytdbot/generate_files.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/generate_json.py` & `Pytdbot-0.8.4.dev1/pytdbot/generate_json.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/handlers/decorators.py` & `Pytdbot-0.8.4.dev1/pytdbot/handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/handlers/handler.py` & `Pytdbot-0.8.4.dev1/pytdbot/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/handlers/updates.py` & `Pytdbot-0.8.4.dev1/pytdbot/handlers/updates.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/methods/methods.py` & `Pytdbot-0.8.4.dev1/pytdbot/methods/methods.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     InlineKeyboardMarkup,
     ShowKeyboardMarkup,
     ForceReply,
     RemoveKeyboard,
     InputFile,
     InputThumbnail,
 )
-from ..utils import is_type
 
 
 class Methods(TDLibFunctions):
     """TDLib API functions class"""
 
     async def sendTextMessage(
         self,
@@ -96,15 +95,15 @@
             _text = {"@type": "formattedText", "text": text, "entities": entities}
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -120,15 +119,15 @@
             "input_message_content": {
                 "@type": "inputMessageText",
                 "text": _text,
                 "disable_web_page_preview": disable_web_page_preview,
                 "clear_draft": clear_draft,
             },
         }
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
         res = await self.invoke(data)
         if res.is_error:
             return res
         _new = Result(data)
         self._results[str(res.result["id"]) + str(res.result["chat_id"])] = _new
         await _new.wait()
@@ -213,23 +212,23 @@
         Returns:
             :class:`~pytdbot.types.Result`
 
         """
 
         parse_mode = parse_mode if parse_mode is not None else self.default_parse_mode
         _caption = None
-        if is_type(caption, str):
+        if isinstance(caption, str):
 
-            if is_type(caption_entities, list):
+            if isinstance(caption_entities, list):
                 _caption = {
                     "@type": "formattedText",
                     "text": caption,
                     "entities": caption_entities,
                 }
-            elif is_type(parse_mode, str):
+            elif isinstance(parse_mode, str):
                 parse = await self.parseText(caption, parse_mode=parse_mode)
                 if parse.is_error:
                     return parse
                 else:
                     _caption = parse.result
             else:
                 _caption = {
@@ -239,15 +238,15 @@
                 }
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -267,28 +266,28 @@
                 "width": width,
                 "height": height,
                 "caption": _caption,
                 "has_spoiler": has_spoiler,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
-        if is_type(animation, InputFile):
+        if isinstance(animation, InputFile):
             data["input_message_content"]["animation"] = animation.to_dict()
-        elif is_type(animation, str):
+        elif isinstance(animation, str):
             data["input_message_content"]["animation"] = {
                 "@type": "inputFileRemote",
                 "id": animation,
             }
         else:
             raise ValueError("animation must be InputFile or str")
 
-        if is_type(thumbnail, InputThumbnail):
+        if isinstance(thumbnail, InputThumbnail):
             data["input_message_content"]["thumbnail"] = thumbnail.to_dict()
 
         res = await self.invoke(data)
         if res.is_error:
             return res
         _new = Result(data)
         self._results[str(res.result["id"]) + str(res.result["chat_id"])] = _new
@@ -367,23 +366,23 @@
         Returns:
             :class:`~pytdbot.types.Result`
 
         """
 
         parse_mode = parse_mode if parse_mode is not None else self.default_parse_mode
         _caption = None
-        if is_type(caption, str):
+        if isinstance(caption, str):
 
-            if is_type(caption_entities, list):
+            if isinstance(caption_entities, list):
                 _caption = {
                     "@type": "formattedText",
                     "text": caption,
                     "entities": caption_entities,
                 }
-            elif is_type(parse_mode, str):
+            elif isinstance(parse_mode, str):
                 parse = await self.parseText(caption, parse_mode=parse_mode)
                 if parse.is_error:
                     return parse
                 else:
                     _caption = parse.result
             else:
                 _caption = {
@@ -393,15 +392,15 @@
                 }
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -419,28 +418,28 @@
                 "title": title,
                 "performer": performer,
                 "duration": duration,
                 "caption": _caption,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
-        if is_type(audio, InputFile):
+        if isinstance(audio, InputFile):
             data["input_message_content"]["audio"] = audio.to_dict()
-        elif is_type(audio, str):
+        elif isinstance(audio, str):
             data["input_message_content"]["audio"] = {
                 "@type": "inputFileRemote",
                 "id": audio,
             }
         else:
             raise ValueError("audio must be InputFile or str")
 
-        if is_type(album_cover_thumbnail, InputThumbnail):
+        if isinstance(album_cover_thumbnail, InputThumbnail):
             data["input_message_content"][
                 "album_cover_thumbnail"
             ] = album_cover_thumbnail.to_dict()
 
         res = await self.invoke(data)
         if res.is_error:
             return res
@@ -512,23 +511,23 @@
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
         parse_mode = parse_mode if parse_mode is not None else self.default_parse_mode
         _caption = None
-        if is_type(caption, str):
+        if isinstance(caption, str):
 
-            if is_type(caption_entities, list):
+            if isinstance(caption_entities, list):
                 _caption = {
                     "@type": "formattedText",
                     "text": caption,
                     "entities": caption_entities,
                 }
-            elif is_type(parse_mode, str):
+            elif isinstance(parse_mode, str):
                 parse = await self.parseText(caption, parse_mode=parse_mode)
                 if parse.is_error:
                     return parse
                 else:
                     _caption = parse.result
             else:
                 _caption = {
@@ -538,15 +537,15 @@
                 }
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -562,28 +561,28 @@
             "input_message_content": {
                 "@type": "inputMessageDocument",
                 "disable_content_type_detection": disable_content_type_detection,
                 "caption": _caption,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
-        if is_type(document, InputFile):
+        if isinstance(document, InputFile):
             data["input_message_content"]["document"] = document.to_dict()
-        elif is_type(document, str):
+        elif isinstance(document, str):
             data["input_message_content"]["document"] = {
                 "@type": "inputFileRemote",
                 "id": document,
             }
         else:
             raise ValueError("document must be InputFile or str")
 
-        if is_type(thumbnail, InputThumbnail):
+        if isinstance(thumbnail, InputThumbnail):
             data["input_message_content"]["thumbnail"] = thumbnail.to_dict()
 
         res = await self.invoke(data)
         if res.is_error:
             return res
         _new = Result(data)
         self._results[str(res.result["id"]) + str(res.result["chat_id"])] = _new
@@ -669,23 +668,23 @@
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
         parse_mode = parse_mode if parse_mode is not None else self.default_parse_mode
         _caption = None
-        if is_type(caption, str):
+        if isinstance(caption, str):
 
-            if is_type(caption_entities, list):
+            if isinstance(caption_entities, list):
                 _caption = {
                     "@type": "formattedText",
                     "text": caption,
                     "entities": caption_entities,
                 }
-            elif is_type(parse_mode, str):
+            elif isinstance(parse_mode, str):
                 parse = await self.parseText(caption, parse_mode=parse_mode)
                 if parse.is_error:
                     return parse
                 else:
                     _caption = parse.result
             else:
                 _caption = {
@@ -695,15 +694,15 @@
                 }
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -723,28 +722,28 @@
                 "height": height,
                 "caption": _caption,
                 "self_destruct_time": self_destruct_time,
                 "has_spoiler": has_spoiler,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
-        if is_type(photo, InputFile):
+        if isinstance(photo, InputFile):
             data["input_message_content"]["photo"] = photo.to_dict()
-        elif is_type(photo, str):
+        elif isinstance(photo, str):
             data["input_message_content"]["photo"] = {
                 "@type": "inputFileRemote",
                 "id": photo,
             }
         else:
             raise ValueError("photo must be InputFile or str")
 
-        if is_type(thumbnail, InputThumbnail):
+        if isinstance(thumbnail, InputThumbnail):
             data["input_message_content"]["thumbnail"] = thumbnail.to_dict()
 
         res = await self.invoke(data)
         if res.is_error:
             return res
         _new = Result(data)
         self._results[str(res.result["id"]) + str(res.result["chat_id"])] = _new
@@ -838,23 +837,23 @@
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
         parse_mode = parse_mode if parse_mode is not None else self.default_parse_mode
         _caption = None
-        if is_type(caption, str):
+        if isinstance(caption, str):
 
-            if is_type(caption_entities, list):
+            if isinstance(caption_entities, list):
                 _caption = {
                     "@type": "formattedText",
                     "text": caption,
                     "entities": caption_entities,
                 }
-            elif is_type(parse_mode, str):
+            elif isinstance(parse_mode, str):
                 parse = await self.parseText(caption, parse_mode=parse_mode)
                 if parse.is_error:
                     return parse
                 else:
                     _caption = parse.result
             else:
                 _caption = {
@@ -864,15 +863,15 @@
                 }
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -894,28 +893,28 @@
                 "height": height,
                 "caption": _caption,
                 "self_destruct_time": self_destruct_time,
                 "has_spoiler": has_spoiler,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
-        if is_type(video, InputFile):
+        if isinstance(video, InputFile):
             data["input_message_content"]["video"] = video.to_dict()
-        elif is_type(video, str):
+        elif isinstance(video, str):
             data["input_message_content"]["video"] = {
                 "@type": "inputFileRemote",
                 "id": video,
             }
         else:
             raise ValueError("video must be InputFile or str")
 
-        if is_type(thumbnail, InputThumbnail):
+        if isinstance(thumbnail, InputThumbnail):
             data["input_message_content"]["thumbnail"] = thumbnail.to_dict()
 
         res = await self.invoke(data)
         if res.is_error:
             return res
         _new = Result(data)
         self._results[str(res.result["id"]) + str(res.result["chat_id"])] = _new
@@ -981,15 +980,15 @@
         """
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -1005,28 +1004,28 @@
             "input_message_content": {
                 "@type": "inputMessageVideoNote",
                 "duration": duration,
                 "length": length,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
-        if is_type(video_note, InputFile):
+        if isinstance(video_note, InputFile):
             data["input_message_content"]["video_note"] = video_note.to_dict()
-        elif is_type(video_note, str):
+        elif isinstance(video_note, str):
             data["input_message_content"]["video_note"] = {
                 "@type": "inputFileRemote",
                 "id": video_note,
             }
         else:
             raise ValueError("video_note must be InputFile or str")
 
-        if is_type(thumbnail, InputThumbnail):
+        if isinstance(thumbnail, InputThumbnail):
             data["input_message_content"]["thumbnail"] = thumbnail.to_dict()
 
         res = await self.invoke(data)
         if res.is_error:
             return res
         _new = Result(data)
         self._results[str(res.result["id"]) + str(res.result["chat_id"])] = _new
@@ -1096,23 +1095,23 @@
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
         parse_mode = parse_mode if parse_mode is not None else self.default_parse_mode
         _caption = None
-        if is_type(caption, str):
+        if isinstance(caption, str):
 
-            if is_type(caption_entities, list):
+            if isinstance(caption_entities, list):
                 _caption = {
                     "@type": "formattedText",
                     "text": caption,
                     "entities": caption_entities,
                 }
-            elif is_type(parse_mode, str):
+            elif isinstance(parse_mode, str):
                 parse = await self.parseText(caption, parse_mode=parse_mode)
                 if parse.is_error:
                     return parse
                 else:
                     _caption = parse.result
             else:
                 _caption = {
@@ -1122,15 +1121,15 @@
                 }
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -1146,23 +1145,23 @@
             "input_message_content": {
                 "@type": "inputMessageVoiceNote",
                 "duration": duration,
                 "caption": _caption,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
-        if is_type(waveform, bytes):
+        if isinstance(waveform, bytes):
             data["input_message_content"]["waveform"] = str(b64encode(waveform))
 
-        if is_type(voice, InputFile):
+        if isinstance(voice, InputFile):
             data["input_message_content"]["voice_note"] = voice.to_dict()
-        elif is_type(voice, str):
+        elif isinstance(voice, str):
             data["input_message_content"]["voice_note"] = {
                 "@type": "inputFileRemote",
                 "id": voice,
             }
         else:
             raise ValueError("voice must be InputFile or str")
 
@@ -1236,15 +1235,15 @@
         """
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -1261,28 +1260,28 @@
                 "@type": "inputMessageSticker",
                 "emoji": emoji,
                 "width": width,
                 "height": height,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
-        if is_type(sticker, InputFile):
+        if isinstance(sticker, InputFile):
             data["input_message_content"]["sticker"] = sticker.to_dict()
-        elif is_type(sticker, str):
+        elif isinstance(sticker, str):
             data["input_message_content"]["sticker"] = {
                 "@type": "inputFileRemote",
                 "id": sticker,
             }
         else:
             raise ValueError("document must be InputFile or str")
 
-        if is_type(thumbnail, InputThumbnail):
+        if isinstance(thumbnail, InputThumbnail):
             data["input_message_content"]["thumbnail"] = thumbnail.to_dict()
 
         res = await self.invoke(data)
         if res.is_error:
             return res
         _new = Result(data)
         self._results[str(res.result["id"]) + str(res.result["chat_id"])] = _new
@@ -1350,23 +1349,23 @@
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
         parse_mode = parse_mode if parse_mode is not None else self.default_parse_mode
         _caption = None
-        if is_type(new_caption, str):
+        if isinstance(new_caption, str):
 
-            if is_type(new_caption_entities, list):
+            if isinstance(new_caption_entities, list):
                 _caption = {
                     "@type": "formattedText",
                     "text": new_caption,
                     "entities": new_caption_entities,
                 }
-            elif is_type(parse_mode, str):
+            elif isinstance(parse_mode, str):
                 parse = await self.parseText(new_caption, parse_mode=parse_mode)
                 if parse.is_error:
                     return parse
                 else:
                     _caption = parse.result
             else:
                 _caption = {
@@ -1376,15 +1375,15 @@
                 }
 
         if load_replied_message == None and not self.use_message_database:
             load_replied_message = True
 
         if (
             load_replied_message == True
-            and is_type(reply_to_message_id, int)
+            and isinstance(reply_to_message_id, int)
             and reply_to_message_id > 0
         ):
             # Because TDLib will ignore `reply_to_message_id`
             # if the message isn't loaded in memory
             await self.getMessage(chat_id, reply_to_message_id)
 
         data = {
@@ -1537,15 +1536,15 @@
             "input_message_content": {
                 "@type": "inputMessageText",
                 "text": _text,
                 "disable_web_page_preview": disable_web_page_preview,
             },
         }
 
-        if is_type(reply_markup, ReplyMarkup):
+        if isinstance(reply_markup, ReplyMarkup):
             data["reply_markup"] = reply_markup.to_dict()
 
         return await self.invoke(data)
 
     async def parseText(
         self,
         text: str,
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/methods/tdlibfunctions.py` & `Pytdbot-0.8.4.dev1/pytdbot/methods/tdlibfunctions.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/td_api.json` & `Pytdbot-0.8.4.dev1/pytdbot/td_api.json`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/td_api.tl` & `Pytdbot-0.8.4.dev1/pytdbot/td_api.tl`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/tdjson/tdjson.py` & `Pytdbot-0.8.4.dev1/pytdbot/tdjson/tdjson.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 from ctypes.util import find_library
 from ctypes import c_int, c_double, c_void_p, c_char_p, CDLL
 from logging import getLogger
 from typing import Union
 from platform import system
 from pkg_resources import resource_filename
-from ujson import loads, dumps
 
+try:
+    import orjson as json
+except ImportError:
+    try:
+        import ujson as json
+    except ImportError:
+        import json
 
 logger = getLogger(__name__)
 
 
+def dumps(obj) -> bytes:
+    if json.__name__ == "orjson":
+        return json.dumps(obj).decode().encode("utf-8")
+    else:
+        return json.dumps(obj).encode("utf-8")
+
+
 class TdJson:
     def __init__(self, lib_path: str = None, verbosity: int = 2) -> None:
         """TdJson client
 
         Args:
             lib_path (``str``, optional):
                 Path to shared library. Defaults to ``None``
@@ -32,15 +45,16 @@
             #     )
             # else:
             lib_path = find_library("tdjson")
 
         if not lib_path:
             raise ValueError("TDLib library not found")
 
-        logger.info("Initializing TdJson client with library: %s", lib_path)
+        logger.debug(f'Using "{json.__name__}" module as JSON encoder')
+        logger.info(f"Initializing TdJson client with library: {lib_path}")
         self._build_client(lib_path, verbosity)
 
     def _build_client(self, lib_path: str, verbosity: int) -> None:
         """Build TdJson client
 
         Args:
             lib_path (``str``):
@@ -73,18 +87,17 @@
         self._td_execute.argtypes = [c_char_p]
 
         self.client_id = self._td_create_client_id()
 
         td_version, td_commit_hash = self.execute(
             {"@type": "getOption", "name": "version"}
         ), self.execute({"@type": "getOption", "name": "commit_hash"})
+
         logger.info(
-            "Using TDLib {} ({})".format(
-                td_version["value"], td_commit_hash["value"][:9]
-            )
+            f"Using TDLib {td_version['value']} ({td_commit_hash['value'][:9]})"
         )
 
         if isinstance(verbosity, int):
             res = self.execute(
                 {"@type": "setLogVerbosityLevel", "new_verbosity_level": verbosity}
             )
 
@@ -99,44 +112,44 @@
                 The maximum number of seconds allowed to wait for new data. Defaults to 2.0
 
         Returns:
             :py:class:``dict``: An incoming update or result to a request. If no data is received, ``None`` is returned
         """
         try:
             if res := self._td_receive(self.client_id, c_double(timeout)):
-                return loads(res.decode("utf-8"))
+                return json.loads(res)
         except Exception:
             logger.exception("Exception while receiving")
             raise
 
     def send(self, data: dict) -> None:
         """Sends a request to TDLib
 
         Args:
             data (``dict``):
                 The request to be sent
         """
         try:
-            self._td_send(self.client_id, dumps(data).encode("utf-8"))
+            self._td_send(self.client_id, dumps(data))
         except Exception:
-            logger.exception("Exception while sending", data)
+            logger.exception(f"Exception while sending: {data}")
             raise
 
     def execute(self, data: dict) -> Union[None, dict]:
         """Executes a TDLib request
 
         Args:
             data (``dict``): The request to be executed
 
         Returns:
             :py:class:``dict``: The result of the request
         """
         try:
-            if res := self._td_execute(dumps(data).encode("utf-8")):
-                return loads(res.decode("utf-8"))
+            if res := self._td_execute(dumps(data)):
+                return json.loads(res)
         except Exception:
             logger.exception("Exception while executing")
             raise
 
     def destroy(self) -> None:
         """Destroys the TDLib client."""
         self._td_client_destroy(self.client_id)
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/__init__.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/__init__.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/buttons/force_reply.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/buttons/force_reply.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/buttons/inline_keyboard.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/buttons/inline_keyboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from base64 import b64encode as b64en
 from .base import ReplyMarkup
-from ...utils import is_type
 
 
 class InlineKeyboardMarkup(ReplyMarkup):
     """Inline keyboard markup"""
 
     def __init__(self, rows: list):
         """Inline keyboard markup
@@ -76,15 +75,15 @@
             data (``bytes``):
                 Data to be sent to the bot via a callback query
 
         Returns:
             :py:class:`dict`
         """
 
-        if is_type(data, str):
+        if isinstance(data, str):
             data = data.encode("utf-8")
 
         return {
             "@type": "inlineKeyboardButton",
             "text": text,
             "type": {
                 "@type": "inlineKeyboardButtonTypeCallback",
@@ -102,15 +101,15 @@
             data (``bytes``):
                 Data to be sent to the bot via a callback query
 
         Returns:
             :py:class:`dict`
         """
 
-        if is_type(data, str):
+        if isinstance(data, str):
             data = data.encode("utf-8")
 
         return {
             "@type": "inlineKeyboardButton",
             "text": text,
             "type": {
                 "@type": "inlineKeyboardButtonTypeCallbackWithPassword",
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/buttons/remove_keyboard.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/buttons/remove_keyboard.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/buttons/show_keyboard.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/buttons/show_keyboard.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_file_generated.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_generated.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_file_local.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_local.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_file_remote.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_remote.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/inputfile/input_thumbnail.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_thumbnail.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/logstream/log_stream_file.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/logstream/log_stream_file.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/result/result.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/result/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from secrets import token_hex
 from asyncio import Event
-from ujson import dumps
+from json import dumps
+import binascii, os
 
 RETRY_AFTER_PREFEX = "Too Many Requests: retry after "
 
 
 class Result:
     """Result object.
 
@@ -14,16 +14,17 @@
 
     """
 
     def __init__(
         self,
         request: dict,
     ) -> None:
-        self.id = token_hex(16)
+        self.id = binascii.hexlify(os.urandom(9)).decode()
         request["@extra"] = {"id": self.id}
+
         self.request = request
         self.is_processed = False
         self.is_error = False
         self.is_limited = False
         self.limited_seconds = 0
         self.result = {}
         self.type = None
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/update/chatActions.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/update/chatActions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytdbot
 from asyncio import sleep
-from ...utils import is_type
+
 
 class ChatActions:
     def __init__(
         self,
         client: "pytdbot.Client",
         chat_id: int,
         action: str,
@@ -12,15 +12,15 @@
     ) -> None:
         self.client = client
         self.chat_id = chat_id
         self.action = None
         self.task = None
         self.message_thread_id = message_thread_id or 0
 
-        assert is_type(self.message_thread_id, int), "message_thread_id must be int"
+        assert isinstance(self.message_thread_id, int), "message_thread_id must be int"
 
         if action == "typing" or action == "chatActionTyping":
             self.action = "chatActionTyping"
         elif action == "upload_photo" or action == "chatActionUploadingPhoto":
             self.action = "chatActionUploadingPhoto"
         elif action == "record_video" or action == "chatActionRecordingVideo":
             self.action = "chatActionRecordingVideo"
@@ -37,15 +37,15 @@
         elif action == "find_location" or action == "chatActionChoosingLocation":
             self.action = "chatActionChoosingLocation"
         elif action == "record_video_note" or action == "chatActionRecordingVideoNote":
             self.action = "chatActionRecordingVideoNote"
         elif action == "upload_video_note" or action == "chatActionUploadingVideoNote":
             self.action = "chatActionUploadingVideoNote"
         else:
-            raise ValueError("Unknown action type {}".format(action))
+            raise ValueError(f"Unknown action type {action}")
 
     async def sendAction(self):
         return await self.client.sendChatAction(
             self.chat_id, self.message_thread_id, {"@type": self.action}
         )
 
     def __await__(self):
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/types/update/update.py` & `Pytdbot-0.8.4.dev1/pytdbot/types/update/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytdbot
 
 from base64 import b64decode
 from typing import Union
-from ujson import dumps
+from json import dumps
 from functools import lru_cache
-from pytdbot.utils import escape_html, escape_markdown, is_type
+from pytdbot.utils import escape_html, escape_markdown
 from pytdbot.types import (
     Result,
     InlineKeyboardMarkup,
     ShowKeyboardMarkup,
     ForceReply,
     RemoveKeyboard,
     InputFile,
@@ -472,29 +472,29 @@
 
         Returns:
             :py:class:`bool`
         """
 
         if self.type == "updateNewMessage":
             return self.update["message"]["sender_id"]["@type"] == "messageSenderUser"
-        elif is_type(self.from_id, int):
+        elif isinstance(self.from_id, int):
             return self.from_id > 0
 
         return False
 
     @property
     @lru_cache(1)
     def is_private(self) -> bool:
         """True, if the update is sent on private chat
 
         Returns:
             :py:class:`bool`
         """
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             return self.chat_id > 0
         return False
 
     @property
     @lru_cache(1)
     def is_service(self) -> bool:
         """True, if the update is service message
@@ -510,15 +510,15 @@
     def is_self(self) -> bool:
         """True, if the message is sent by the current user
 
         Returns:
             :py:class:`bool`
         """
 
-        if is_type(self.from_id, int):
+        if isinstance(self.from_id, int):
             return self.client.options["my_id"] == self.from_id
         return False
 
     async def mention(self, parse_mode: str = "markdown", version: int = 2) -> str:
         """Get the text_mention of the message sender
 
         Args:
@@ -545,15 +545,15 @@
                     return f"[{escape_markdown(name, version=version)}](tg://user?id={self.from_id})"
 
     async def getRepliedMessage(
         self,
     ) -> Result:
         """Get the replied message"""
 
-        if is_type(self.message_id, int):
+        if isinstance(self.message_id, int):
             return await self.client.getRepliedMessage(
                 self.chat_id,
                 self.message_id,
             )
 
     async def getMessage(
         self,
@@ -564,29 +564,29 @@
         Args:
             message_id (``int``, *optional*):
                 The message id, If ``None``, :meth:`~pytdbot.types.Update.message_id` is used
         """
 
         message_id = message_id or self.message_id
 
-        if is_type(message_id, int):
+        if isinstance(message_id, int):
             return await self.client.getMessage(self.chat_id, message_id)
 
     async def getChat(
         self,
     ) -> Result:
         """Get chat info"""
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             return await self.client.getChat(self.chat_id)
 
     async def getChatMember(self) -> Result:
         """Get member info in the current chat"""
 
-        if is_type(self.chat_id, int) and is_type(self.from_id, int):
+        if isinstance(self.chat_id, int) and isinstance(self.from_id, int):
             if self.is_user:
                 member_id = {"@type": "messageSenderUser", "user_id": self.from_id}
             else:
                 member_id = {"@type": "messageSenderChat", "chat_id": self.from_id}
             return await self.client.getChatMember(self.chat_id, member_id=member_id)
 
     async def getUser(
@@ -623,15 +623,15 @@
             only_for_self (``bool``, *optional*):
                 True, if the message needs to be pinned for one side only; private chats only
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
-        if is_type(self.message_id, int):
+        if isinstance(self.message_id, int):
             return await self.client.pinChatMessage(
                 self.chat_id,
                 self.message_id,
                 disable_notification,
                 only_for_self,
             )
 
@@ -645,15 +645,15 @@
             revoke (``bool``, *optional*):
                 Pass true to delete messages for all chat members. Always true for supergroups, channels and secret chats
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
-        if is_type(self.message_id, int):
+        if isinstance(self.message_id, int):
             return await self.client.deleteMessages(
                 self.chat_id, [self.message_id], revoke
             )
 
     async def leaveChat(self, chat_id: int = None) -> Result:
         """Leave the current chat
 
@@ -661,15 +661,15 @@
             chat_id (``int``, *optional*):
                 The chat to leave. Defaults to the current chat
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
-        chat_id = chat_id if is_type(chat_id, int) else self.chat_id
+        chat_id = chat_id if isinstance(chat_id, int) else self.chat_id
 
         if chat_id:
             return await self.client.leaveChat(chat_id)
 
     def action(self, action: str, message_thread_id: int = None) -> ChatActions:
         """Sends a chat action to a specific chat. Supporting context manager (``with`` statment)
 
@@ -699,15 +699,15 @@
             message_thread_id (``int``, *optional*):
                 If not 0, a message thread identifier in which the action was performed. Defaults to ``None``
 
         Returns:
             :class:`~pytdbot.types.ChatActions`
         """
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return ChatActions(self.client, self.chat_id, action, message_thread_id)
         else:
             raise ValueError("Unknown chat_id")
 
     async def download(self, file_id: int = None) -> Result:
         """Download the current received media
@@ -717,15 +717,15 @@
                 File identifier to download. Defaults to None (:meth:`~pytdbot.types.Update.local_file_id`)
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
         file_id = file_id or self.local_file_id
-        if is_type(file_id, int):
+        if isinstance(file_id, int):
             return await self.client.downloadFile(
                 file_id, priority=1, offset=None, limit=None, synchronous=True
             )
 
     async def answerCallbackQuery(
         self,
         text: str,
@@ -781,17 +781,17 @@
             disable_notification (``bool``, *optional*):
                 If True, disable notification for the message
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
-        if (is_type(self.message_id, int) or is_type(message_id, int)) and is_type(
-            self.chat_id, int
-        ):
+        if (
+            isinstance(self.message_id, int) or isinstance(message_id, int)
+        ) and isinstance(self.chat_id, int):
             return await self.client.forwardMessage(
                 chat_id,
                 self.chat_id,
                 message_id or self.message_id,
                 in_game_share,
                 disable_notification,
             )
@@ -873,15 +873,15 @@
                 reply_to_message_id = self.message_id
             else:
                 if self.is_private:
                     reply_to_message_id = 0
                 else:
                     reply_to_message_id = self.message_id
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return await self.client.sendTextMessage(
                 self.chat_id,
                 text,
                 entities=entities,
                 parse_mode=parse_mode,
                 disable_web_page_preview=disable_web_page_preview,
@@ -990,15 +990,15 @@
                 reply_to_message_id = self.message_id
             else:
                 if self.is_private:
                     reply_to_message_id = 0
                 else:
                     reply_to_message_id = self.message_id
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return await self.client.sendAnimation(
                 self.chat_id,
                 animation,
                 thumbnail=thumbnail,
                 caption=caption,
                 caption_entities=caption_entities,
@@ -1104,15 +1104,15 @@
                 reply_to_message_id = self.message_id
             else:
                 if self.is_private:
                     reply_to_message_id = 0
                 else:
                     reply_to_message_id = self.message_id
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return await self.client.sendAudio(
                 self.chat_id,
                 audio,
                 caption=caption,
                 caption_entities=caption_entities,
                 parse_mode=parse_mode,
@@ -1204,15 +1204,15 @@
                 reply_to_message_id = self.message_id
             else:
                 if self.is_private:
                     reply_to_message_id = 0
                 else:
                     reply_to_message_id = self.message_id
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return await self.client.sendDocument(
                 self.chat_id,
                 document,
                 caption=caption,
                 caption_entities=caption_entities,
                 parse_mode=parse_mode,
@@ -1293,15 +1293,15 @@
                 reply_to_message_id = self.message_id
             else:
                 if self.is_private:
                     reply_to_message_id = 0
                 else:
                     reply_to_message_id = self.message_id
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return await self.client.sendSticker(
                 self.chat_id,
                 sticker,
                 emoji=emoji,
                 disable_notification=disable_notification,
                 protect_content=protect_content,
@@ -1404,15 +1404,15 @@
                 reply_to_message_id = self.message_id
             else:
                 if self.is_private:
                     reply_to_message_id = 0
                 else:
                     reply_to_message_id = self.message_id
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return await self.client.sendVideo(
                 self.chat_id,
                 video,
                 duration=duration,
                 width=width,
                 height=height,
@@ -1505,15 +1505,15 @@
                 reply_to_message_id = self.message_id
             else:
                 if self.is_private:
                     reply_to_message_id = 0
                 else:
                     reply_to_message_id = self.message_id
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return await self.client.sendPhoto(
                 self.chat_id,
                 photo,
                 caption=caption,
                 caption_entities=caption_entities,
                 parse_mode=parse_mode,
@@ -1606,15 +1606,15 @@
                 reply_to_message_id = self.message_id
             else:
                 if self.is_private:
                     reply_to_message_id = 0
                 else:
                     reply_to_message_id = self.message_id
 
-        if is_type(self.chat_id, int):
+        if isinstance(self.chat_id, int):
             message_thread_id = message_thread_id or self.message_thread_id
             return await self.client.sendVoice(
                 self.chat_id,
                 voice,
                 caption=caption,
                 caption_entities=caption_entities,
                 parse_mode=parse_mode,
@@ -1672,15 +1672,15 @@
             reply_markup (:class:`~pytdbot.types.InlineKeyboardMarkup` | :class:`~pytdbot.types.ShowKeyboardMarkup` | :class:`~pytdbot.types.ForceReply` | :class:`~pytdbot.types.RemoveKeyboard`, *optional*):
                 The message reply markup
 
         Returns:
             :class:`~pytdbot.types.Result`
         """
 
-        if is_type(self.message_id, int):
+        if isinstance(self.message_id, int):
             return await self.client.editTextMessage(
                 self.chat_id,
                 self.message_id,
                 text,
                 entities=entities,
                 parse_mode=parse_mode,
                 disable_web_page_preview=disable_web_page_preview,
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/utils/escape.py` & `Pytdbot-0.8.4.dev1/pytdbot/utils/escape.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from html import escape as _html_escape
-from re import escape as _re_escape, compile as _re_compile
+import re
 
 
 def escape_html(text: str, quote: bool = True) -> str:
     """Escape HTML characters in the given text
 
     Args:
         text (``str``):
@@ -15,16 +15,16 @@
     Returns:
         :py:class:`str`: The escaped text
     """
 
     return _html_escape(text, quote=quote)
 
 
-special_chars_v1 = _re_compile("([{}])".format(_re_escape(r"_\*`\[")))
-special_chars_v2 = _re_compile("([{}])".format(_re_escape(r"\_*[]()~`>#+-=|{}.!")))
+special_chars_v1 = re.compile("([{}])".format(re.escape(r"_\*`\[")))
+special_chars_v2 = re.compile("([{}])".format(re.escape(r"\_*[]()~`>#+-=|{}.!")))
 
 
 def escape_markdown(text: str, version: int = 2) -> str:
     """Escape Markdown characters in the given text
 
     Args:
         text (``str``):
```

### Comparing `Pytdbot-0.8.4.dev0/pytdbot/utils/text_format.py` & `Pytdbot-0.8.4.dev1/pytdbot/utils/text_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import escape_html, escape_markdown, is_type
+from . import escape_html, escape_markdown
 
 
 def bold(text: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to bold format
 
     Args:
         text (``str``):
@@ -15,17 +15,17 @@
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
     if html:
-        return "<b>{}</b>".format(text if escape is False else escape_html(text))
+        return f"<b>{text if escape is False else escape_html(text)}</b>"
     else:
-        return "*{}*".format(text if escape is False else escape_markdown(text))
+        return f"*{text if escape is False else escape_markdown(text)}*"
 
 
 def italic(text: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to italic format
 
     Args:
         text (``str``):
@@ -38,17 +38,17 @@
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
     if html:
-        return "<i>{}</i>".format(text if escape is False else escape_html(text))
+        return f"<i>{text if escape is False else escape_html(text)}</i>"
     else:
-        return "_{}_".format(text if escape is False else escape_markdown(text))
+        return f"_{text if escape is False else escape_markdown(text)}_"
 
 
 def underline(text: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to underline format
 
     Args:
         text (``str``):
@@ -61,17 +61,17 @@
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
     if html:
-        return "<u>{}</u>".format(text if escape is False else escape_html(text))
+        return f"<u>{text if escape is False else escape_html(text)}</u>"
     else:
-        return "__{}__".format(text if escape is False else escape_markdown(text))
+        return f"__{text if escape is False else escape_markdown(text)}__"
 
 
 def strikethrough(text: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to strikethrough format
 
     Args:
         text (``str``):
@@ -84,17 +84,17 @@
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
     if html:
-        return "<s>{}</s>".format(text if escape is False else escape_html(text))
+        return f"<s>{text if escape is False else escape_html(text)}</s>"
     else:
-        return "~{}~".format(text if escape is False else escape_markdown(text))
+        return f"~{text if escape is False else escape_markdown(text)}~"
 
 
 def spoiler(text: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to spoiler format
 
     Args:
         text (``str``):
@@ -107,19 +107,17 @@
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
     if html:
-        return '<span class="tg-spoiler">{}</span>'.format(
-            text if escape is False else escape_html(text)
-        )
+        return f'<span class="tg-spoiler">{text if escape is False else escape_html(text)}</span>'
     else:
-        return "||{}||".format(text if escape is False else escape_markdown(text))
+        return f"||{text if escape is False else escape_markdown(text)}||"
 
 
 def hyperlink(text: str, url: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to hyperlink format
 
     Args:
         text (``str``):
@@ -134,24 +132,20 @@
         escape (``bool``, *optional*):
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
-    assert is_type(url, str), "url must be str"
+    assert isinstance(url, str), "url must be str"
 
     if html:
-        return '<a href="{}">{}</a>'.format(
-            url, text if escape is False else escape_html(text)
-        )
+        return f'<a href="{url}">{text if escape is False else escape_html(text)}</a>'
     else:
-        return "[{}]({})".format(
-            text if escape is False else escape_markdown(text), url
-        )
+        return f"[{text if escape is False else escape_markdown(text)}]({url})"
 
 
 def mention(text: str, user_id: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to inline mention format
 
     Args:
         text (``str``):
@@ -167,21 +161,17 @@
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
     if html:
-        return '<a href="tg://user?id={}">{}</a>'.format(
-            user_id, text if escape is False else escape_html(text)
-        )
+        return f'<a href="tg://user?id={user_id}">{text if escape is False else escape_html(text)}</a>'
     else:
-        return "[{}](tg://user?id={})".format(
-            text if escape is False else escape_markdown(text), user_id
-        )
+        return f"[{text if escape is False else escape_markdown(text)}](tg://user?id={user_id})"
 
 
 def code(text: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to code format
 
     Args:
         text (``str``):
@@ -194,17 +184,17 @@
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
     if html:
-        return "<code>{}</code>".format(text if escape is False else escape_html(text))
+        return f"<code>{text if escape is False else escape_html(text)}</code>"
     else:
-        return "`{}`".format(text if escape is False else escape_markdown(text))
+        return f"`{text if escape is False else escape_markdown(text)}`"
 
 
 def pre(text: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to pre format
 
     Args:
         text (``str``):
@@ -217,17 +207,17 @@
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
     if html:
-        return "<pre>{}</pre>".format(text if escape is False else escape_html(text))
+        return f"<pre>{text if escape is False else escape_html(text)}</pre>"
     else:
-        return "```\n{}\n```".format(text if escape is False else escape_markdown(text))
+        return f"```\n{text if escape is False else escape_markdown(text)}\n```"
 
 
 def pre_code(text: str, language: str, html: bool = False, escape: bool = True) -> str:
     """Convert the given text to pre code format
 
     Args:
         text (``str``):
@@ -242,17 +232,15 @@
         escape (``bool``, *optional*):
             Whether escape special characters to the given text or not. Defaults to ``True``
 
     Returns:
         :py:class:`str`: The formated text
     """
 
-    assert is_type(language, str), "text must be str"
+    assert isinstance(language, str), "text must be str"
 
     if html:
-        return '<pre><code class="language-{}">{}</code></pre>'.format(
-            language, text if escape is False else escape_html(text)
-        )
+        return f'<pre><code class="language-{language}">{text if escape is False else escape_html(text)}</code></pre>'
     else:
-        return "```{}\n{}\n```".format(
-            language, text if escape is False else escape_markdown(text)
+        return (
+            f"```{language}\n{text if escape is False else escape_markdown(text)}\n```"
         )
```

### Comparing `Pytdbot-0.8.4.dev0/setup.py` & `Pytdbot-0.8.4.dev1/setup.py`

 * *Files identical despite different names*

