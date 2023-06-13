# Comparing `tmp/blaster-server-0.0.436b0.tar.gz` & `tmp/blaster-server-0.0.437.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.436b0.tar", last modified: Wed Jun  7 13:55:26 2023, max compression
+gzip compressed data, was "blaster-server-0.0.437.tar", last modified: Tue Jun 13 09:57:46 2023, max compression
```

## Comparing `blaster-server-0.0.436b0.tar` & `blaster-server-0.0.437.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.436b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/cloud/aws/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.436b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/connection_pool.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.436b0/blaster/env.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.436b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62732 2023-06-05 22:08:59.000000 blaster-server-0.0.436b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15679 2023-06-07 13:51:59.000000 blaster-server-0.0.436b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38804 2023-06-07 13:55:11.000000 blaster-server-0.0.436b0/blaster/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/tools/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46341 2023-06-05 22:16:59.000000 blaster-server-0.0.436b0/blaster/tools/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/utils/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/data/mime_types.json
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/fork.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/lat_long_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3953 2023-06-06 19:29:14.000000 blaster-server-0.0.436b0/blaster/utils/phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/websocket/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_app.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_core.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_exceptions.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_handshake.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_http.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_logging.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_socket.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_ssl_compat.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_url.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_utils.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/websocket/tests/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/tests/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster_server.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1726 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/examples/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/fast_api_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/gevent_wsgi_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/meinheld_flask.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/simple_examples.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/test_chat_room.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/tornado_hello_world.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/wheezy_hello.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1531 2023-06-07 13:52:37.000000 blaster-server-0.0.436b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/test/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/test/test_schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5954 2023-06-05 22:21:25.000000 blaster-server-0.0.436b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/test/test_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.099030 blaster-server-0.0.437/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.437/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.437/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-13 09:57:46.099030 blaster-server-0.0.437/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.437/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.437/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.437/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.437/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.437/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.437/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.437/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.437/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62732 2023-06-05 22:08:59.000000 blaster-server-0.0.437/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15679 2023-06-07 13:51:59.000000 blaster-server-0.0.437/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38833 2023-06-09 14:07:27.000000 blaster-server-0.0.437/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    43823 2023-06-13 08:38:49.000000 blaster-server-0.0.437/blaster/tools/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.437/blaster/tools/sanitize_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.437/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3953 2023-06-06 19:29:14.000000 blaster-server-0.0.437/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.099030 blaster-server-0.0.437/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-13 09:57:46.099030 blaster-server-0.0.437/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-06-09 14:09:20.000000 blaster-server-0.0.437/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.099030 blaster-server-0.0.437/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.437/test/test_command_line_parser.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.437/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.437/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.437/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.437/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.437/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.437/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.436b0/LICENSE.txt` & `blaster-server-0.0.437/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/PKG-INFO` & `blaster-server-0.0.437/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.436b0
+Version: 0.0.437
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.436b0/README.md` & `blaster-server-0.0.437/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/__init__.py` & `blaster-server-0.0.437/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/cloud/analytics.py` & `blaster-server-0.0.437/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.437/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.437/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/cloud/storage.py` & `blaster-server-0.0.437/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/config.py` & `blaster-server-0.0.437/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/connection_pool.py` & `blaster-server-0.0.437/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/env.py` & `blaster-server-0.0.437/blaster/env.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/logging.py` & `blaster-server-0.0.437/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/mongo_orm.py` & `blaster-server-0.0.437/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/schema.py` & `blaster-server-0.0.437/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/server.py` & `blaster-server-0.0.437/blaster/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import inspect
 import socket
 from gevent.socket import socket as GeventSocket
 from gevent.server import StreamServer
 from requests_toolbelt.multipart import decoder
 
 from . import req_ctx
-from .tools import SanitizedDict,\
-	set_socket_fast_close_options, BufferedSocket, ltrim,\
-	_OBJ_END_
+from .tools import set_socket_fast_close_options,\
+	BufferedSocket, ltrim, _OBJ_END_
+from .tools.sanitize_html import SanitizedDict
 from .utils import events
 from .utils.data_utils import FILE_EXTENSION_TO_MIME_TYPE
 from .logging import LOG_ERROR, LOG_SERVER, LOG_WARN, LOG_DEBUG
 from .schema import Int, Object, Required, schema as schema_func
 from .websocket.server import WebSocketServerHandler
 from .config import IS_DEV, BLASTER_HTTP_TOOK_LONG_WARN_THRESHOLD
 
@@ -347,15 +347,15 @@
 	@classmethod
 	def arg_generator(cls, name, _type, default):
 		if(_type in (str, int, float)):
 			return lambda req: (_type(_val) if _val != None else None)\
 				if (_val := req.get(name, default)) != _OBJ_END_\
 				else raise_ex(
 					MissingBlasterArgumentException(name, _type)
-				)
+			)
 		elif(_type == Request):  # req: Request
 			return lambda req: req
 		elif(_type == Query):  # query: Query
 			return lambda req: req._params
 		elif(_type == Headers):  # headers: Headers
 			return lambda req: req._headers
 		elif(_type == Body):  # headers: Headers
@@ -801,15 +801,15 @@
 		request_type = None
 		request_path = None
 		headers = None
 		try:
 			request_line = request_line.decode("utf-8")
 			request_type, _request_line = request_line.split(" ", 1)
 			# set request type
-			req.request_type = request_type 
+			req.request_type = request_type
 			_http_protocol_index = _request_line.rfind(" ")
 			request_path \
 				= req.path \
 				= _request_line[: _http_protocol_index]
 			# special issue, seeing request path will full domain name
 			if(request_path.startswith("http")):
 				if(
@@ -1219,15 +1219,15 @@
 		os.path.join(dp, f)
 		for dp, dn, filenames in os.walk(_base_folder_path_) for f in filenames
 	]
 	for file_name in file_names:
 		relative_file_path = ltrim(file_name, _base_folder_path_)
 		_url_file_path = url_path + relative_file_path
 		# strip / at the begininning in the cache
-		# as we search matching path without leading slash in the cache 
+		# as we search matching path without leading slash in the cache
 		# in the file handler
 		file_cache[_url_file_path] = get_file_resp(relative_file_path)
 
 	return url_path + "{*path}", file_handler
 
 
 def proxy_file_handler(url_path, proxy_url):
@@ -1249,15 +1249,15 @@
 
 
 Request.set_arg_type_hook(WebSocketServerHandler, _get_web_socket_handler)
 
 
 # Utils
 
-MOBILE_USER_AGENT_REGEX = re.compile(r"(android|bb\\d+|meego).+mobile|avantgo|bada\\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|mobile.+firefox|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\\.(browser|link)|vodafone|wap|windows ce|xda|xiino", re.I|re.M)
+MOBILE_USER_AGENT_REGEX = re.compile(r"(android|bb\\d+|meego).+mobile|avantgo|bada\\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|mobile.+firefox|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\\.(browser|link)|vodafone|wap|windows ce|xda|xiino", re.I | re.M)
 
 MOBILE_USER_AGENT_REGEX2 = re.compile(r"1207|6310|6590|3gso|4thp|50[1-6]i|770s|802s|a wa|abac|ac(er|oo|s\\-)|ai(ko|rn)|al(av|ca|co)|amoi|an(ex|ny|yw)|aptu|ar(ch|go)|as(te|us)|attw|au(di|\\-m|r |s )|avan|be(ck|ll|nq)|bi(lb|rd)|bl(ac|az)|br(e|v)w|bumb|bw\\-(n|u)|c55\\/|capi|ccwa|cdm\\-|cell|chtm|cldc|cmd\\-|co(mp|nd)|craw|da(it|ll|ng)|dbte|dc\\-s|devi|dica|dmob|do(c|p)o|ds(12|\\-d)|el(49|ai)|em(l2|ul)|er(ic|k0)|esl8|ez([4-7]0|os|wa|ze)|fetc|fly(\\-|_)|g1 u|g560|gene|gf\\-5|g\\-mo|go(\\.w|od)|gr(ad|un)|haie|hcit|hd\\-(m|p|t)|hei\\-|hi(pt|ta)|hp( i|ip)|hs\\-c|ht(c(\\-| |_|a|g|p|s|t)|tp)|hu(aw|tc)|i\\-(20|go|ma)|i230|iac( |\\-|\\/)|ibro|idea|ig01|ikom|im1k|inno|ipaq|iris|ja(t|v)a|jbro|jemu|jigs|kddi|keji|kgt( |\\/)|klon|kpt |kwc\\-|kyo(c|k)|le(no|xi)|lg( g|\\/(k|l|u)|50|54|\\-[a-w])|libw|lynx|m1\\-w|m3ga|m50\\/|ma(te|ui|xo)|mc(01|21|ca)|m\\-cr|me(rc|ri)|mi(o8|oa|ts)|mmef|mo(01|02|bi|de|do|t(\\-| |o|v)|zz)|mt(50|p1|v )|mwbp|mywa|n10[0-2]|n20[2-3]|n30(0|2)|n50(0|2|5)|n7(0(0|1)|10)|ne((c|m)\\-|on|tf|wf|wg|wt)|nok(6|i)|nzph|o2im|op(ti|wv)|oran|owg1|p800|pan(a|d|t)|pdxg|pg(13|\\-([1-8]|c))|phil|pire|pl(ay|uc)|pn\\-2|po(ck|rt|se)|prox|psio|pt\\-g|qa\\-a|qc(07|12|21|32|60|\\-[2-7]|i\\-)|qtek|r380|r600|raks|rim9|ro(ve|zo)|s55\\/|sa(ge|ma|mm|ms|ny|va)|sc(01|h\\-|oo|p\\-)|sdk\\/|se(c(\\-|0|1)|47|mc|nd|ri)|sgh\\-|shar|sie(\\-|m)|sk\\-0|sl(45|id)|sm(al|ar|b3|it|t5)|so(ft|ny)|sp(01|h\\-|v\\-|v )|sy(01|mb)|t2(18|50)|t6(00|10|18)|ta(gt|lk)|tcl\\-|tdg\\-|tel(i|m)|tim\\-|t\\-mo|to(pl|sh)|ts(70|m\\-|m3|m5)|tx\\-9|up(\\.b|g1|si)|utst|v400|v750|veri|vi(rg|te)|vk(40|5[0-3]|\\-v)|vm40|voda|vulc|vx(52|53|60|61|70|80|81|83|85|98)|w3c(\\-| )|webc|whit|wi(g |nc|nw)|wmlb|wonu|x700|yas\\-|your|zeto|zte\\-", re.I | re.M)
 
 
 def is_mobile_user_agent(user_agent):
 	return MOBILE_USER_AGENT_REGEX.search(user_agent) \
 		or MOBILE_USER_AGENT_REGEX2.search(user_agent[0:4])
```

### Comparing `blaster-server-0.0.436b0/blaster/tools/__init__.py` & `blaster-server-0.0.437/blaster/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 @author: abhinav
 '''
 
 from gevent.threading import Thread
 from gevent.queue import Queue
 import os
 import sys
+import weakref
 import subprocess
 import shlex
 import collections
 import random
 import string
 import socket
 import struct
 import fcntl
-import html
 import heapq
 from gevent import sleep
 from functools import reduce as _reduce
 from gevent.lock import BoundedSemaphore
 from datetime import timezone
 from datetime import datetime
 from datetime import timedelta
@@ -882,17 +882,17 @@
 	return [item for item in first if item not in second]
 
 
 # what are added vs what need to be deleted from first
 # no order
 def list_diff2(first, second, key=None):
 	if(not first and second):
-		return [], second
+		return [], list(second)
 	if(second == None):
-		return first, []
+		return list(first), []
 	if(key):
 		second_keys = set(map(key, second))
 		first_keys = set(map(key, first))
 		# to add and delete
 		return [item for item in first if key(item) not in second_keys],\
 			[item for item in second if key(item) not in first_keys]
 	else:
@@ -1091,124 +1091,14 @@
 		if len(current_batch) == n:
 			yield current_batch
 			current_batch = []
 	if current_batch:
 		yield current_batch
 
 
-# custom containers ##########
-# SanitizedList and SanitizedDict are used for HTML safe operation
-# the idea is to wrap them to sanitizeContainers while inserting
-# rather than retrieving
-
-class SanitizedSetterGetter(object):
-	def __getitem__(self, k, escape_quotes=True, escape_html=True):
-		val = super().__getitem__(k)
-		if(escape_html and isinstance(val, str)):
-			# make it html safe
-			return html.escape(val, quote=escape_quotes)
-		return val
-
-	def __setitem__(self, key, val):
-		if(isinstance(val, dict)):
-			new_val = SanitizedDict()
-			for k, v in val.items():
-				new_val[k] = v  # calls __setitem__ nested way
-			super().__setitem__(key, new_val)
-
-		elif(isinstance(val, list)):
-			new_val = SanitizedList()
-			for i in val:
-				new_val.append(i)
-			super().__setitem__(key, new_val)
-		else:
-			super().__setitem__(key, val)
-
-
-class SanitizedList(SanitizedSetterGetter, list):
-
-	def __iter__(self):
-		# unoptimized but for this it's okay, always returns sanitized one
-		def sanitized(val):
-			if(isinstance(val, str)):
-				return html.escape(val, quote=True)
-			return val
-		return map(sanitized, list.__iter__(self))
-
-	def at(self, k, escape_quotes=True, escape_html=True):
-		self.__getitem__(
-			k,
-			escape_quotes=escape_quotes,
-			escape_html=escape_html
-		)
-
-	def extend(self, _list):
-		for val in _list:
-			# calls __setitem__ again
-			self.append(val)
-		# allow chaining
-		return self
-
-	def append(self, val):
-		if(isinstance(val, dict)):
-			new_val = SanitizedDict()
-			for k, v in val.items():
-				new_val[k] = v  # calls __setitem__ nested way
-			super().append(new_val)
-
-		elif(isinstance(val, list)):
-			new_val = SanitizedList()
-			for i in val:
-				new_val.append(i)
-			super().append(new_val)
-		else:
-			super().append(val)
-		# allow chaining
-		return self
-
-
-# intercepts all values setting and
-class SanitizedDict(SanitizedSetterGetter, dict):
-	# can pass escape_html=false if you want raw data
-	def get(self, key, default=None, escape_html=True, escape_quotes=True):
-		try:
-			val = self.__getitem__(
-				key,
-				escape_html=escape_html,
-				escape_quotes=escape_quotes
-			)
-			return val
-		except KeyError:
-			return default
-
-	def items(self):
-		# unoptimized but for this it's okay, always returns sanitized one
-		def sanitized(key_val):
-			key, val = key_val
-			if(isinstance(val, str)):
-				return (key, html.escape(val, quote=True))
-			return key_val
-		return map(sanitized, dict.items(self))
-
-	def update(self, another):
-		for k, v in another.items():
-			# calls __setitem__ again
-			self[k] = v
-		# allow chaining
-		return self
-
-
-class LowerKeyDict(dict):
-	def __getitem__(self, k):
-		return super().__getitem__(k.lower())
-
-	def get(self, k, default=None):
-		return super().get(k.lower(), default)
-
-
 # This is the most *important* socket wrapped implementation
 # used by blaster server.
 class BufferedSocket():
 
 	is_eof = False
 	sock = None
 	store = None
@@ -1416,48 +1306,38 @@
 			self.lock.release()
 		return
 
 
 def parse_cmd_line_arguments():
 	from sys import argv
 	args = []
-	args_map = {
-		"args": args
-	}
+	args_map = {}
 	i = 0
 	num_args = len(argv)
 	while(i < num_args):
 		arg = argv[i]
-		if(arg.startswith("--")):
+		if(arg.startswith("-")):
 			if("=" in arg):
 				key, val = arg.split("=", 1)
 				args_map[key.lstrip("-")] = val
 			else:
-				args_map[arg.lstrip("-")] = True
-		elif(arg.startswith("-")):  # Flags
-			key = arg.lstrip("-")
-			# if next argument doesn't start with - its considered as value
-			val = True
-			if (i + 1 < num_args and argv[i + 1][0] != "-"):
-				val = argv[i + 1]
-				i += 1
-			args_map[key] = val
+				next_arg = True
+				if(i + 1 < num_args and not argv[i + 1].startswith("-")):
+					next_arg = argv[i + 1]
+					i += 1
+				args_map[arg.lstrip("-")] = next_arg
 		else:
 			args.append(arg)
 
 		i += 1
-	return args_map
+	return args, args_map
 
 
 # PARSE COMMAND LINE ARGUMENTS BY DEFAULT
-CommandLineArgs = parse_cmd_line_arguments()
-
-
-# PARSE COMMAND LINE ARGUMENTS BY DEFAULT
-CommandLineArgs = parse_cmd_line_arguments()
+CommandLineArgs, CommandLineNamedArgs = parse_cmd_line_arguments()
 
 
 def run_shell(cmd, output_parser=None, shell=False, max_buf=5000, fail=True, state=None, env=None, **kwargs):
 
 	DEBUG_PRINT_LEVEL > 2 and print(f"#RUNNING: {cmd}")
 	state = state if state != None else DummyObject()
 	state.total_output = ""
@@ -1851,7 +1731,23 @@
 			os.remove(cache_file_path)
 
 	bytes_buffer = BytesIO(open(cache_file_path, "rb").read())
 	if(as_string_buffer):
 		return StringIO(bytes_buffer.read().decode())
 	else:
 		return bytes_buffer
+
+
+def memoized_method(func):
+	cache = {}
+
+	def wrapper(self, *args, **kwargs):
+		# need weakref otherwise cache will never be garbage collected
+		key = (weakref.ref(self), args, frozenset(kwargs.items()))
+		if key in cache:
+			return cache[key]
+		result = func(self, *args, **kwargs)
+		cache[key] = result
+		return result
+	setattr(wrapper, "_original", func)
+	wrapper.clear_cache = cache.clear
+	return wrapper
```

### Comparing `blaster-server-0.0.436b0/blaster/utils/data/countries.json` & `blaster-server-0.0.437/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.437/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/utils/data_utils.py` & `blaster-server-0.0.437/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/utils/events.py` & `blaster-server-0.0.437/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/utils/fork.py` & `blaster-server-0.0.437/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.437/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.437/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/utils/xss_html.py` & `blaster-server-0.0.437/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/__init__.py` & `blaster-server-0.0.437/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.437/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_app.py` & `blaster-server-0.0.437/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_core.py` & `blaster-server-0.0.437/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.437/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.437/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_http.py` & `blaster-server-0.0.437/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_logging.py` & `blaster-server-0.0.437/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_socket.py` & `blaster-server-0.0.437/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.437/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_url.py` & `blaster-server-0.0.437/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/_utils.py` & `blaster-server-0.0.437/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/server.py` & `blaster-server-0.0.437/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.437/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.437/blaster_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.436b0
+Version: 0.0.437
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.436b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.437/blaster_server.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 blaster/cloud/__init__.py
 blaster/cloud/analytics.py
 blaster/cloud/push_tasks.py
 blaster/cloud/storage.py
 blaster/cloud/aws/__init__.py
 blaster/cloud/aws/ses_utils.py
 blaster/tools/__init__.py
+blaster/tools/sanitize_html.py
 blaster/utils/__init__.py
 blaster/utils/data_utils.py
 blaster/utils/events.py
 blaster/utils/fork.py
 blaster/utils/lat_long_utils.py
 blaster/utils/phone_number_utils.py
 blaster/utils/xss_html.py
@@ -54,13 +55,14 @@
 examples/meinheld_flask.py
 examples/mongo_ormexample.py
 examples/simple_examples.py
 examples/test_chat_room.py
 examples/tornado_hello_world.py
 examples/wheezy_hello.py
 test/__init__.py
+test/test_command_line_parser.py
 test/test_mongo_orm.py
 test/test_phone_number_utils.py
 test/test_schema.py
 test/test_tools.py
 test/test_utils.py
 test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.436b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.437/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/examples/mongo_ormexample.py` & `blaster-server-0.0.437/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/examples/simple_examples.py` & `blaster-server-0.0.437/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/examples/test_chat_room.py` & `blaster-server-0.0.437/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/examples/tornado_hello_world.py` & `blaster-server-0.0.437/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/examples/wheezy_hello.py` & `blaster-server-0.0.437/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/setup.py` & `blaster-server-0.0.437/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.436b',
+	version='0.0.437',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.436b0/test/test_mongo_orm.py` & `blaster-server-0.0.437/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/test/test_phone_number_utils.py` & `blaster-server-0.0.437/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/test/test_schema.py` & `blaster-server-0.0.437/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/test/test_tools.py` & `blaster-server-0.0.437/test/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from blaster import tools
 import time
 from blaster.tools import get_time_overlaps, retry,\
-	SanitizedDict, SanitizedList, ExpiringCache,\
-	create_signed_value, decode_signed_value
+	ExpiringCache, create_signed_value, decode_signed_value
+from blaster.tools.sanitize_html import SanitizedDict, SanitizedList
 from datetime import datetime
 from blaster.utils.data_utils import parse_string_to_units,\
 	parse_currency_string
 
 
 class TestSanitization(unittest.TestCase):
 	def test_sanitization(self):
```

### Comparing `blaster-server-0.0.436b0/test/test_utils.py` & `blaster-server-0.0.437/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436b0/test/timeit_snippets.py` & `blaster-server-0.0.437/test/timeit_snippets.py`

 * *Files identical despite different names*

