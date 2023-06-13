# Comparing `tmp/fast_tracker-0.2.89.tar.gz` & `tmp/fast_tracker-0.2.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fast_tracker-0.2.89.tar", last modified: Mon Apr 10 08:07:25 2023, max compression
+gzip compressed data, was "dist/fast_tracker-0.2.90.tar", last modified: Tue Jun 13 09:03:35 2023, max compression
```

## Comparing `fast_tracker-0.2.89.tar` & `fast_tracker-0.2.90.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/
--rw-r--r--   0 songh02   (1000) songh02   (1000)    13333 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/apache-skywalking-LICENSE
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/agent/
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/agent/protocol/
--rw-r--r--   0 songh02   (1000) songh02   (1000)      920 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/agent/protocol/udp.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      375 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/agent/protocol/__init__.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3553 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/agent/__init__.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      696 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/FastTracker.json
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/bootstrap/
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3909 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/bootstrap/sitecustomize.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      103 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/bootstrap/__init__.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1827 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/decorators.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/admin/
--rw-r--r--   0 songh02   (1000) songh02   (1000)      134 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/admin/__main__.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3092 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/admin/run_python.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3291 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/admin/run_program.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3772 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/admin/__init__.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/report/
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1869 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/report/report_struct.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      103 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/report/__init__.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/plugins/
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3141 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_urllib3.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     2153 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_urllib_request.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     2765 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_rq.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     4839 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_django.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     4992 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_http_server.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3753 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_kafka.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     2882 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_requests.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1097 2023-04-10 07:00:39.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_pymysql.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1295 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_elasticsearch.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     2908 2023-04-07 08:35:58.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_rabbitmq.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1156 2023-04-10 06:43:23.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_mysqldb.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     5959 2023-04-07 08:43:46.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_falcon.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1116 2023-04-10 03:20:40.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_redis.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     4247 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_pymongo.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     4556 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_flask.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3243 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/__init__.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     8856 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_tornado.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     4261 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/plugins/fast_log.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)    12244 2023-04-10 03:12:52.000000 fast_tracker-0.2.89/fast_tracker/config.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1135 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/loggings.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     9291 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/fast_tracker.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/client/
--rw-r--r--   0 songh02   (1000) songh02   (1000)     6394 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/client/udp.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      383 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/client/__init__.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/utils/
--rw-r--r--   0 songh02   (1000) songh02   (1000)      565 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/utils/lang.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      122 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/utils/exceptions.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1644 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/utils/counter.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      244 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/utils/reader_type.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1135 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/utils/functions.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      785 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/utils/__init__.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     4232 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/fast_tracker_configer.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/trace/
--rw-r--r--   0 songh02   (1000) songh02   (1000)      654 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/tags.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     7726 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/span.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     2603 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/segment.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     4297 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/carrier.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker/trace/ipc/
--rw-r--r--   0 songh02   (1000) songh02   (1000)      653 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/ipc/process.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)        1 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/ipc/__init__.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      906 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/snapshot.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     7042 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/context.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)      361 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/fast_tracker/trace/__init__.py
--rw-r--r--   0 songh02   (1000) songh02   (1000)     2077 2023-04-07 09:22:58.000000 fast_tracker-0.2.89/fast_tracker/__init__.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/scripts/
--rwxr-xr-x   0 songh02   (1000) songh02   (1000)      320 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/scripts/fast-boot
--rw-r--r--   0 songh02   (1000) songh02   (1000)       38 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/setup.cfg
--rw-r--r--   0 songh02   (1000) songh02   (1000)     3022 2023-04-10 06:59:25.000000 fast_tracker-0.2.89/setup.py
-drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker.egg-info/
--rw-r--r--   0 songh02   (1000) songh02   (1000)       13 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker.egg-info/top_level.txt
--rw-r--r--   0 songh02   (1000) songh02   (1000)        1 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 songh02   (1000) songh02   (1000)       55 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker.egg-info/entry_points.txt
--rw-r--r--   0 songh02   (1000) songh02   (1000)     2042 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 songh02   (1000) songh02   (1000)      106 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker.egg-info/requires.txt
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1537 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/fast_tracker.egg-info/PKG-INFO
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1537 2023-04-10 08:07:25.000000 fast_tracker-0.2.89/PKG-INFO
--rw-r--r--   0 songh02   (1000) songh02   (1000)     1001 2023-04-07 07:14:56.000000 fast_tracker-0.2.89/README.rst
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)    13333 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/apache-skywalking-LICENSE
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/agent/
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/agent/protocol/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      920 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/agent/protocol/udp.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      375 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/agent/protocol/__init__.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3553 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/agent/__init__.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      696 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/FastTracker.json
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/bootstrap/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3909 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/bootstrap/sitecustomize.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      103 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/bootstrap/__init__.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1827 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/decorators.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/admin/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      134 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/admin/__main__.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3092 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/admin/run_python.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3291 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/admin/run_program.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3772 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/admin/__init__.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/report/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1869 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/report/report_struct.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      103 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/report/__init__.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/plugins/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3141 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_urllib3.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     2153 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_urllib_request.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     2765 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_rq.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     4839 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_django.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     4992 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_http_server.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3753 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_kafka.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3160 2023-06-06 08:35:01.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_requests.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1097 2023-04-10 07:00:39.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_pymysql.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1295 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_elasticsearch.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     2908 2023-04-07 08:35:58.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_rabbitmq.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1156 2023-04-10 06:43:23.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_mysqldb.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     5959 2023-06-06 08:41:55.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_falcon.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1116 2023-04-10 03:20:40.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_redis.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     4247 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_pymongo.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     4556 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_flask.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3243 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/__init__.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     8856 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_tornado.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     4261 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/plugins/fast_log.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)    12244 2023-04-10 03:12:52.000000 fast_tracker-0.2.90/fast_tracker/config.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1135 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/loggings.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     9291 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/fast_tracker.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/client/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     6394 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/client/udp.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      383 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/client/__init__.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/utils/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      565 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/utils/lang.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      122 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/utils/exceptions.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1644 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/utils/counter.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      244 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/utils/reader_type.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1135 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/utils/functions.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      785 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/utils/__init__.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     4232 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/fast_tracker_configer.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/trace/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      683 2023-06-06 07:35:53.000000 fast_tracker-0.2.90/fast_tracker/trace/tags.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     7726 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/trace/span.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     2603 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/trace/segment.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     4307 2023-06-06 03:53:11.000000 fast_tracker-0.2.90/fast_tracker/trace/carrier.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker/trace/ipc/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      653 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/trace/ipc/process.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)        1 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/trace/ipc/__init__.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      906 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/trace/snapshot.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     7042 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/trace/context.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      361 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/fast_tracker/trace/__init__.py
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     2077 2023-04-07 09:22:58.000000 fast_tracker-0.2.90/fast_tracker/__init__.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/scripts/
+-rwxr-xr-x   0 songh02   (1000) songh02   (1000)      320 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/scripts/fast-boot
+-rw-r--r--   0 songh02   (1000) songh02   (1000)       38 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/setup.cfg
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     3022 2023-06-06 06:57:01.000000 fast_tracker-0.2.90/setup.py
+drwxr-xr-x   0 songh02   (1000) songh02   (1000)        0 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker.egg-info/
+-rw-r--r--   0 songh02   (1000) songh02   (1000)       13 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker.egg-info/top_level.txt
+-rw-r--r--   0 songh02   (1000) songh02   (1000)        1 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 songh02   (1000) songh02   (1000)       55 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     2042 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 songh02   (1000) songh02   (1000)      106 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker.egg-info/requires.txt
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1537 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/fast_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1537 2023-06-13 09:03:35.000000 fast_tracker-0.2.90/PKG-INFO
+-rw-r--r--   0 songh02   (1000) songh02   (1000)     1001 2023-04-07 07:14:56.000000 fast_tracker-0.2.90/README.rst
```

### Comparing `fast_tracker-0.2.89/apache-skywalking-LICENSE` & `fast_tracker-0.2.90/apache-skywalking-LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/agent/protocol/udp.py` & `fast_tracker-0.2.90/fast_tracker/agent/protocol/udp.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/agent/__init__.py` & `fast_tracker-0.2.90/fast_tracker/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/FastTracker.json` & `fast_tracker-0.2.90/fast_tracker/FastTracker.json`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/bootstrap/sitecustomize.py` & `fast_tracker-0.2.90/fast_tracker/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/decorators.py` & `fast_tracker-0.2.90/fast_tracker/decorators.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/admin/run_python.py` & `fast_tracker-0.2.90/fast_tracker/admin/run_python.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/admin/run_program.py` & `fast_tracker-0.2.90/fast_tracker/admin/run_program.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/admin/__init__.py` & `fast_tracker-0.2.90/fast_tracker/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/report/report_struct.py` & `fast_tracker-0.2.90/fast_tracker/report/report_struct.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_urllib3.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_urllib3.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_urllib_request.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_urllib_request.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_rq.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_rq.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_django.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_django.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_http_server.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_http_server.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_kafka.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_kafka.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_requests.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,26 +61,33 @@
                 stream,
                 verify,
                 cert,
                 json,
             )
 
         context = get_context()
+        trace_id_name = config.get_trace_id_name()
+        trace_id = ""
         with context.new_exit_span(op=url_param.path or "/", peer=url_param.netloc) as span:
             carrier = span.inject()
             span.layer = Layer.Http
             span.component = ComponentType.Requests
 
             if headers is None:
                 headers = {}
             for item in carrier:
+                if getattr(item, "trace_id", None):
+                    trace_id = item.trace_id
                 headers[item.key] = item.val
 
+            headers[trace_id_name] = trace_id
+
             span.tag(Tag(key=tags.HttpMethod, val=method.upper()))
             span.tag(Tag(key=tags.HttpUrl, val=url))
+            span.tag(Tag(key=tags.HttpHeaders, val=headers))
             # HttpPath 只需要获取PATH_INFO信息即可，不需要？后的内容
             span.tag(Tag(key=tags.HttpPath, val=url_param.path))
 
             res = _request(
                 this,
                 method,
                 url,
```

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_pymysql.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_pymysql.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_elasticsearch.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_rabbitmq.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_mysqldb.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_mysqldb.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_falcon.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_falcon.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_redis.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_redis.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_pymongo.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_pymongo.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_flask.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_flask.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/__init__.py` & `fast_tracker-0.2.90/fast_tracker/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_tornado.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_tornado.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/plugins/fast_log.py` & `fast_tracker-0.2.90/fast_tracker/plugins/fast_log.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/config.py` & `fast_tracker-0.2.90/fast_tracker/config.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/loggings.py` & `fast_tracker-0.2.90/fast_tracker/loggings.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/fast_tracker.py` & `fast_tracker-0.2.90/fast_tracker/fast_tracker.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/client/udp.py` & `fast_tracker-0.2.90/fast_tracker/client/udp.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/utils/lang.py` & `fast_tracker-0.2.90/fast_tracker/utils/lang.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/utils/counter.py` & `fast_tracker-0.2.90/fast_tracker/utils/counter.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/utils/functions.py` & `fast_tracker-0.2.90/fast_tracker/utils/functions.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/utils/__init__.py` & `fast_tracker-0.2.90/fast_tracker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/fast_tracker_configer.py` & `fast_tracker-0.2.90/fast_tracker/fast_tracker_configer.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/trace/tags.py` & `fast_tracker-0.2.90/fast_tracker/trace/tags.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 # http
 HttpUrl = "url"
 HttpPath = "path"
 HttpMethod = "http_method"
 HttpStatus = "status_code"
 HttpParams = "http_params"
+HttpHeaders = "http_headers"
 
 # db
 DbType = "db_type"
 DbInstance = "db_instance"
 DbStatement = "db_statement"
 DbSqlParameters = "db_sql_parameters"
```

### Comparing `fast_tracker-0.2.89/fast_tracker/trace/span.py` & `fast_tracker-0.2.90/fast_tracker/trace/span.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/trace/segment.py` & `fast_tracker-0.2.90/fast_tracker/trace/segment.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/trace/carrier.py` & `fast_tracker-0.2.90/fast_tracker/trace/carrier.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,19 +62,19 @@
 
     @property
     def val(self) -> str:
         return "-".join(
             [
                 b64encode(self.trace_id),
                 self.span_id,
-                b64encode(self.segment_id),
-                b64encode(self.service),
-                b64encode(self.service_instance),
-                b64encode(self.endpoint),
-                b64encode(self.client_address),
+                # b64encode(self.segment_id),
+                # b64encode(self.service),
+                # b64encode(self.service_instance),
+                # b64encode(self.endpoint),
+                # b64encode(self.client_address),
             ]
         )
 
     @val.setter
     def val(self, val: str):
         self.__val = val
         if not val:
```

### Comparing `fast_tracker-0.2.89/fast_tracker/trace/ipc/process.py` & `fast_tracker-0.2.90/fast_tracker/trace/ipc/process.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/trace/snapshot.py` & `fast_tracker-0.2.90/fast_tracker/trace/snapshot.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/trace/context.py` & `fast_tracker-0.2.90/fast_tracker/trace/context.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker/__init__.py` & `fast_tracker-0.2.90/fast_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/setup.py` & `fast_tracker-0.2.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: System :: Monitoring",
 ]
 
 kwargs = dict(
     name="fast_tracker",
-    version="0.2.89",
+    version="0.2.90",
     description=f"FAST Python Agent\n. latest git commit id: {get_latest_git_hash()}",
     long_description=open(readme_file).read(),
     url="http://doc.mypaas.com.cn/fast/03_%E6%9C%8D%E5%8A%A1%E7%AB%AF%E6%8E%A2%E9%92%88%E9%9B%86%E6%88%90/%E7%AE%80%E4%BB%8B.html",
     author="FAST",
     author_email="duanyy03@mingyuanyun.com",
     maintainer="FAST",
     maintainer_email="duanyy03@mingyuanyun.com",
```

### Comparing `fast_tracker-0.2.89/fast_tracker.egg-info/SOURCES.txt` & `fast_tracker-0.2.90/fast_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_tracker-0.2.89/fast_tracker.egg-info/PKG-INFO` & `fast_tracker-0.2.90/fast_tracker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tracker
-Version: 0.2.89
+Version: 0.2.90
 Summary: FAST Python Agent
 Home-page: http://doc.mypaas.com.cn/fast/03_%E6%9C%8D%E5%8A%A1%E7%AB%AF%E6%8E%A2%E9%92%88%E9%9B%86%E6%88%90/%E7%AE%80%E4%BB%8B.html
 Author: FAST
 Author-email: duanyy03@mingyuanyun.com
 Maintainer: FAST
 Maintainer-email: duanyy03@mingyuanyun.com
 License: Apache-2.0
```

### Comparing `fast_tracker-0.2.89/PKG-INFO` & `fast_tracker-0.2.90/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tracker
-Version: 0.2.89
+Version: 0.2.90
 Summary: FAST Python Agent
 Home-page: http://doc.mypaas.com.cn/fast/03_%E6%9C%8D%E5%8A%A1%E7%AB%AF%E6%8E%A2%E9%92%88%E9%9B%86%E6%88%90/%E7%AE%80%E4%BB%8B.html
 Author: FAST
 Author-email: duanyy03@mingyuanyun.com
 Maintainer: FAST
 Maintainer-email: duanyy03@mingyuanyun.com
 License: Apache-2.0
```

### Comparing `fast_tracker-0.2.89/README.rst` & `fast_tracker-0.2.90/README.rst`

 * *Files identical despite different names*

