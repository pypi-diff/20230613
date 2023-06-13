# Comparing `tmp/ipapp-1.3.9.tar.gz` & `tmp/ipapp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipapp-1.3.9.tar", max compression
+gzip compressed data, was "ipapp-2.0.0.tar", max compression
```

## Comparing `ipapp-1.3.9.tar` & `ipapp-2.0.0.tar`

### file list

```diff
@@ -1,82 +1,81 @@
--rw-r--r--   0        0        0     1085 2022-07-06 14:22:54.552915 ipapp-1.3.9/LICENSE
--rw-r--r--   0        0        0     1050 2022-07-06 14:22:54.552915 ipapp-1.3.9/README.md
--rw-r--r--   0        0        0      679 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/__init__.py
--rw-r--r--   0        0        0     6049 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/app.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/asgi/__init__.py
--rw-r--r--   0        0        0     8014 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/asgi/uvicorn.py
--rw-r--r--   0        0        0     3652 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/autoreload.py
--rw-r--r--   0        0        0     4407 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/cli.py
--rw-r--r--   0        0        0      690 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/component.py
--rw-r--r--   0        0        0     9744 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/config.py
--rw-r--r--   0        0        0     6930 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/ctx.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/db/__init__.py
--rw-r--r--   0        0        0    22205 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/db/oracle.py
--rw-r--r--   0        0        0    39149 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/db/pg.py
--rw-r--r--   0        0        0      158 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/error.py
--rw-r--r--   0        0        0      268 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/http/__init__.py
--rw-r--r--   0        0        0     5581 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/http/_base.py
--rw-r--r--   0        0        0     5290 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/http/client.py
--rw-r--r--   0        0        0    14968 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/http/server.py
--rw-r--r--   0        0        0     3259 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/__init__.py
--rw-r--r--   0        0        0      472 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/__init__.py
--rw-r--r--   0        0        0      810 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/_abc.py
--rw-r--r--   0        0        0     5180 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/prometheus.py
--rw-r--r--   0        0        0    18741 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/requests.py
--rw-r--r--   0        0        0     1351 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/sentry.py
--rw-r--r--   0        0        0     3065 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/zipkin.py
--rw-r--r--   0        0        0     3163 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/logger.py
--rw-r--r--   0        0        0    14493 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/span.py
--rw-r--r--   0        0        0     6111 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/misc.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/mq/__init__.py
--rw-r--r--   0        0        0    32899 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/mq/pika.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/openapi/__init__.py
--rw-r--r--   0        0        0     8694 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/openapi/misc.py
--rw-r--r--   0        0        0    10428 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/openapi/models.py
--rw-r--r--   0        0        0     2879 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/openapi/templates.py
--rw-r--r--   0        0        0      210 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/__init__.py
--rw-r--r--   0        0        0       66 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/const.py
--rw-r--r--   0        0        0      124 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/error.py
--rw-r--r--   0        0        0      294 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/http/__init__.py
--rw-r--r--   0        0        0     2599 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/http/client.py
--rw-r--r--   0        0        0    15026 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/http/server.py
--rw-r--r--   0        0        0      173 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/__init__.py
--rw-r--r--   0        0        0      880 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/error.py
--rw-r--r--   0        0        0      424 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/http/__init__.py
--rw-r--r--   0        0        0     2352 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/http/client.py
--rw-r--r--   0        0        0     5719 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/http/server.py
--rw-r--r--   0        0        0    23314 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/main.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/mq/__init__.py
--rw-r--r--   0        0        0     8451 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/mq/pika.py
--rw-r--r--   0        0        0       51 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/__init__.py
--rw-r--r--   0        0        0    11725 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/discover.py
--rw-r--r--   0        0        0     5853 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/models.py
--rw-r--r--   0        0        0    17002 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/main.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/mq/__init__.py
--rw-r--r--   0        0        0    10032 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/mq/pika.py
--rw-r--r--   0        0        0      495 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/__init__.py
--rw-r--r--   0        0        0     2488 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/error.py
--rw-r--r--   0        0        0      424 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/http/__init__.py
--rw-r--r--   0        0        0     2235 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/http/client.py
--rw-r--r--   0        0        0    19283 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/http/server.py
--rw-r--r--   0        0        0    18441 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/main.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/openapi/__init__.py
--rw-r--r--   0        0        0     9426 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/openapi/misc.py
--rw-r--r--   0        0        0      136 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/s3/__init__.py
--rw-r--r--   0        0        0    20855 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/s3/boto.py
--rw-r--r--   0        0        0       90 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/s3/exceptions.py
--rw-r--r--   0        0        0     5293 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/s3/models.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/sftp/__init__.py
--rw-r--r--   0        0        0    17841 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/sftp/client.py
--rw-r--r--   0        0        0       56 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/sphinx/__init__.py
--rw-r--r--   0        0        0     4115 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/sphinx/config.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/task/__init__.py
--rw-r--r--   0        0        0    39913 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/task/db.py
--rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/__init__.py
--rw-r--r--   0        0        0       69 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/__init__.py
--rw-r--r--   0        0        0     1223 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/local.py
--rw-r--r--   0        0        0     3643 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/main.py
--rw-r--r--   0        0        0     4350 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/pg.py
--rw-r--r--   0        0        0     5804 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/redis.py
--rw-r--r--   0        0        0     3680 2022-07-06 14:23:30.787729 ipapp-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     3585 2022-07-06 14:23:31.479622 ipapp-1.3.9/setup.py
--rw-r--r--   0        0        0     4326 2022-07-06 14:23:31.480138 ipapp-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-13 11:00:20.186944 ipapp-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1050 2023-06-13 11:00:20.186944 ipapp-2.0.0/README.md
+-rw-r--r--   0        0        0      679 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/app.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/asgi/__init__.py
+-rw-r--r--   0        0        0     8079 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/asgi/uvicorn.py
+-rw-r--r--   0        0        0     3668 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/autoreload.py
+-rw-r--r--   0        0        0     4407 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/cli.py
+-rw-r--r--   0        0        0      690 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/component.py
+-rw-r--r--   0        0        0     9744 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/config.py
+-rw-r--r--   0        0        0     6930 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/ctx.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/db/__init__.py
+-rw-r--r--   0        0        0    22205 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/db/oracle.py
+-rw-r--r--   0        0        0    39149 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/db/pg.py
+-rw-r--r--   0        0        0      158 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/error.py
+-rw-r--r--   0        0        0      268 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/http/__init__.py
+-rw-r--r--   0        0        0     5748 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/http/_base.py
+-rw-r--r--   0        0        0     5829 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/http/client.py
+-rw-r--r--   0        0        0    16861 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/http/server.py
+-rw-r--r--   0        0        0     3259 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/__init__.py
+-rw-r--r--   0        0        0      471 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/__init__.py
+-rw-r--r--   0        0        0      810 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/_abc.py
+-rw-r--r--   0        0        0     5180 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/prometheus.py
+-rw-r--r--   0        0        0    18741 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/requests.py
+-rw-r--r--   0        0        0     1351 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/sentry.py
+-rw-r--r--   0        0        0     3065 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/zipkin.py
+-rw-r--r--   0        0        0     3163 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/logger.py
+-rw-r--r--   0        0        0    14493 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/span.py
+-rw-r--r--   0        0        0     6111 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/misc.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/mq/__init__.py
+-rw-r--r--   0        0        0    32905 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/mq/pika.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/openapi/__init__.py
+-rw-r--r--   0        0        0     8694 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/openapi/misc.py
+-rw-r--r--   0        0        0    10428 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/openapi/models.py
+-rw-r--r--   0        0        0     2879 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/openapi/templates.py
+-rw-r--r--   0        0        0      210 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/__init__.py
+-rw-r--r--   0        0        0       66 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/const.py
+-rw-r--r--   0        0        0      124 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/error.py
+-rw-r--r--   0        0        0      294 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/http/__init__.py
+-rw-r--r--   0        0        0     2599 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/http/client.py
+-rw-r--r--   0        0        0    15026 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/http/server.py
+-rw-r--r--   0        0        0      173 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/__init__.py
+-rw-r--r--   0        0        0      880 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/error.py
+-rw-r--r--   0        0        0      424 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/http/__init__.py
+-rw-r--r--   0        0        0     2352 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/http/client.py
+-rw-r--r--   0        0        0     5450 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/http/server.py
+-rw-r--r--   0        0        0    23360 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/main.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/mq/__init__.py
+-rw-r--r--   0        0        0     8451 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/mq/pika.py
+-rw-r--r--   0        0        0       51 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/__init__.py
+-rw-r--r--   0        0        0    11725 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/discover.py
+-rw-r--r--   0        0        0     5853 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/models.py
+-rw-r--r--   0        0        0    17002 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/main.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/mq/__init__.py
+-rw-r--r--   0        0        0    10032 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/mq/pika.py
+-rw-r--r--   0        0        0      495 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/__init__.py
+-rw-r--r--   0        0        0     2488 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/error.py
+-rw-r--r--   0        0        0      424 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/http/__init__.py
+-rw-r--r--   0        0        0     2235 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/http/client.py
+-rw-r--r--   0        0        0    19028 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/http/server.py
+-rw-r--r--   0        0        0    18406 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/main.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/openapi/__init__.py
+-rw-r--r--   0        0        0     9426 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/openapi/misc.py
+-rw-r--r--   0        0        0      136 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/s3/__init__.py
+-rw-r--r--   0        0        0    20855 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/s3/boto.py
+-rw-r--r--   0        0        0       90 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/s3/exceptions.py
+-rw-r--r--   0        0        0     5293 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/s3/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/sftp/__init__.py
+-rw-r--r--   0        0        0    17841 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/sftp/client.py
+-rw-r--r--   0        0        0       56 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/sphinx/__init__.py
+-rw-r--r--   0        0        0     4115 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/sphinx/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/task/__init__.py
+-rw-r--r--   0        0        0    39913 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/task/db.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/__init__.py
+-rw-r--r--   0        0        0       69 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/__init__.py
+-rw-r--r--   0        0        0     1223 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/local.py
+-rw-r--r--   0        0        0     3643 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/main.py
+-rw-r--r--   0        0        0     4350 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/pg.py
+-rw-r--r--   0        0        0     5804 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/redis.py
+-rw-r--r--   0        0        0     3893 2023-06-13 11:00:58.663153 ipapp-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4615 1970-01-01 00:00:00.000000 ipapp-2.0.0/PKG-INFO
```

### Comparing `ipapp-1.3.9/LICENSE` & `ipapp-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/README.md` & `ipapp-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/__init__.py` & `ipapp-2.0.0/ipapp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.0'
+__version__ = '2.0.0'
 __build_stamp__ = 0
 
 from . import app, error
 from .app import BaseApplication
 from .cli import main
 from .component import Component
 from .config import BaseConfig
```

### Comparing `ipapp-1.3.9/ipapp/app.py` & `ipapp-2.0.0/ipapp/app.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,16 @@
 
         self.log_info('Running...')
 
     async def stop(self) -> None:
         self.log_info('Shutting down...')
         for comp_name in self._components:
             await self._stop_comp(comp_name)
-        await self.loop.shutdown_asyncgens()
         await self._stop_logger()
+        await self.loop.shutdown_asyncgens()
 
     def shutdown(self) -> None:
         self._shutdown_fut.set_result(None)
 
     def restart(self) -> None:
         self._shutdown_fut.set_result(RESTART)
```

### Comparing `ipapp-1.3.9/ipapp/asgi/uvicorn.py` & `ipapp-2.0.0/ipapp/asgi/uvicorn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import logging
+import re
 import ssl
 from contextvars import Token
 from functools import partial
 from typing import Any, Awaitable, Callable, Dict, Optional, Tuple
 from urllib.parse import parse_qs
 
 from fastapi.applications import FastAPI
@@ -12,18 +13,21 @@
 from uvicorn.config import LOGGING_CONFIG, SSL_PROTOCOL_VERSION
 from uvicorn.main import Config, Server
 from yarl import URL
 
 from ipapp.component import Component
 from ipapp.ctx import span
 from ipapp.http import HttpSpan
-from ipapp.http._base import RE_SECRET_WORDS
 from ipapp.http.server import ServerHttpSpan
 from ipapp.misc import ctx_span_reset, ctx_span_set
 
+RE_SECRET_WORDS = re.compile(
+    "(pas+wo?r?d|pass(phrase)?|pwd|token|secrete?)", re.IGNORECASE
+)
+
 
 class UvicornConfig(BaseModel):
     host: str = "127.0.0.1"
     port: int = 8000
     uds: Optional[str] = None
     fd: Optional[int] = None
     loop: str = "auto"
```

### Comparing `ipapp-1.3.9/ipapp/autoreload.py` & `ipapp-2.0.0/ipapp/autoreload.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from typing import List, Optional, Union
 
 try:
     from watchdog import observers
     from watchdog.events import FileSystemEvent
 except ImportError:
-    observers = None
+    observers = None  # type: ignore
 
 
 _has_execv: bool = sys.platform != 'win32'
 _reload_attempted: bool = False
 
 
 class EventHandler(object):
```

### Comparing `ipapp-1.3.9/ipapp/cli.py` & `ipapp-2.0.0/ipapp/cli.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/component.py` & `ipapp-2.0.0/ipapp/component.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/config.py` & `ipapp-2.0.0/ipapp/config.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/ctx.py` & `ipapp-2.0.0/ipapp/ctx.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/db/oracle.py` & `ipapp-2.0.0/ipapp/db/oracle.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 https://oracle.github.io/odpi/doc/installation.html#linux
 
 https://cx-oracle.readthedocs.io/en/latest/user_guide/introduction.html
 
 https://container-registry.oracle.com/pls/apex/f?p=113:4:103772846430850::NO:::
 """
 import asyncio
-from contextvars import Token
 import functools
+from contextvars import Token
 from typing import Any, Callable, List, Optional, Type, Union
 
 import cx_Oracle
 from pydantic import BaseModel, Field
 
 from ipapp.component import Component
 from ipapp.error import PrepareError
```

### Comparing `ipapp-1.3.9/ipapp/db/pg.py` & `ipapp-2.0.0/ipapp/db/pg.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/http/_base.py` & `ipapp-2.0.0/ipapp/http/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-import re
 import warnings
-from typing import Optional
+from typing import Optional, Tuple, Union
 
 from multidict import MultiMapping
 from yarl import URL
 
 import ipapp.app  # noqa
 import ipapp.misc as misc
 from ipapp.logger.span import Span
 
-RE_SECRET_WORDS = re.compile(
-    "(pas+wo?r?d|pass(phrase)?|pwd|token|secrete?)", re.IGNORECASE
-)
-
 
 class ClientServerAnnotator:
     app: 'ipapp.app.BaseApplication'
+    _secret_keys: Optional[Tuple[str]] = None
 
-    @staticmethod
-    def _mask_url(url: URL) -> str:
+    def _mask_url(self, url: URL) -> str:
         if url.password:
             url = url.with_password('***')
-        for key, val in url.query.items():
-            if RE_SECRET_WORDS.match(key):
-                url = url.update_query({key: '***'})
+        query = url.query
+        if query and self._secret_keys:
+            keys_to_upd = {}
+            for key_mask in self._secret_keys:
+                if key_mask in query:
+                    keys_to_upd[key_mask] = '***'
+            url = url.update_query(keys_to_upd)
         return str(url)
 
     def _span_annotate_req_hdrs(
         self, span: 'HttpSpan', headers: MultiMapping[str], ts: float
     ) -> None:
         try:
             hdrs = '\r\n'.join('%s: %s' % (k, v) for k, v in headers.items())
@@ -38,21 +37,23 @@
 
         except Exception as err:
             self.app.log_err(err)
 
     def _span_annotate_req_body(
         self,
         span: 'HttpSpan',
-        body: Optional[bytes],
+        body: Optional[Union[dict, bytes]],
         ts: float,
         encoding: Optional[str] = None,
     ) -> None:
         try:
             if body is None:
                 content = ''
+            elif isinstance(body, dict):
+                content = str(body)
             else:
                 content = self._decode_bytes(body, encoding=encoding)
 
             span.annotate(HttpSpan.ANN_REQUEST_BODY, content, ts)
             self._span_ann_format4zipkin(
                 span, HttpSpan.ANN_REQUEST_BODY, content, ts
             )
```

### Comparing `ipapp-1.3.9/ipapp/http/client.py` & `ipapp-2.0.0/ipapp/http/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import re
 import time
 from ssl import SSLContext
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, Union
 
+import aiohttp.hdrs
 from aiohttp import ClientResponse, ClientSession, ClientTimeout
 from aiohttp.typedefs import StrOrURL
 from pydantic import BaseModel, Field
 from yarl import URL
 
 import ipapp
 from ipapp.component import Component
@@ -66,46 +67,47 @@
         return super().finish(ts, exception)
 
 
 class Client(Component, ClientServerAnnotator):
     # TODO make pool of clients
 
     cfg = ClientConfig()
+    _session: ClientSession
 
     def __init__(
         self,
         cfg: Optional[ClientConfig] = None,
         json_encode: Callable[[Any], str] = default_json_encode,
         session_kwargs: Optional[Dict[str, Any]] = None,
     ):
-        _session_kwargs = session_kwargs or {}
-        timeout = getattr(cfg, 'timeout', None)
-        if timeout:
-            _session_kwargs.update({'timeout': ClientTimeout(timeout)})
-
         if cfg is not None:
             self.cfg = cfg
         self._json_encode = json_encode
-        self._session = ClientSession(**_session_kwargs)
+        self._session_kwargs = session_kwargs
 
     async def prepare(self) -> None:
         pass
 
     async def start(self) -> None:
-        pass
+        _session_kwargs = self._session_kwargs or {}
+        timeout = getattr(self.cfg, 'timeout', None)
+        if timeout:
+            _session_kwargs.update({'timeout': ClientTimeout(timeout)})
+        self._session = ClientSession(**_session_kwargs)
 
     async def stop(self) -> None:
-        pass
+        await self._session.close()
 
     async def request(
         self,
         method: str,
         url: StrOrURL,
         *,
-        body: Optional[bytes] = None,
+        body: Optional[Union[dict, bytes]] = None,
+        log_body: Optional[Union[dict, bytes]] = None,
         headers: Dict[str, str] = None,
         timeout: Optional[ClientTimeout] = None,
         ssl: Optional[SSLContext] = None,
         request_kwargs: Optional[Dict[str, Any]] = None,
         propagate_trace: bool = True,
     ) -> ClientResponse:
         span: 'ClientHttpSpan'
@@ -115,18 +117,14 @@
             if not isinstance(url, URL):
                 url = URL(url)
 
             span.tag(HttpSpan.TAG_HTTP_URL, self._mask_url(url))
             span.tag(HttpSpan.TAG_HTTP_HOST, url.host)
             span.tag(HttpSpan.TAG_HTTP_METHOD, method)
             span.tag(HttpSpan.TAG_HTTP_PATH, url.path)
-            if body is not None:
-                span.tag(HttpSpan.TAG_HTTP_REQUEST_SIZE, len(body))
-            else:
-                span.tag(HttpSpan.TAG_HTTP_REQUEST_SIZE, 0)
 
             if timeout is None:
                 timeout = ClientTimeout()
 
             if headers is None:
                 headers = {}
             if propagate_trace:
@@ -141,27 +139,44 @@
                 data=body,
                 headers=headers,
                 ssl=ssl,
                 timeout=timeout,
                 **(request_kwargs or {}),
             ) as resp:
                 ts2 = time.time()
+
+                if body is not None:
+                    span.tag(
+                        HttpSpan.TAG_HTTP_REQUEST_SIZE,
+                        resp.request_info.headers.getone(
+                            aiohttp.hdrs.CONTENT_LENGTH, "0"
+                        ),
+                    )
+
                 if self.cfg.log_req_hdrs:
                     self._span_annotate_req_hdrs(
                         span, resp.request_info.headers, ts1
                     )
                 if self.cfg.log_req_body:
-                    self._span_annotate_req_body(span, body, ts1)
+                    if log_body is None:
+                        log_body = body
+                    self._span_annotate_req_body(span, log_body, ts1)
                 if self.cfg.log_resp_hdrs:
                     self._span_annotate_resp_hdrs(span, resp.headers, ts2)
 
-                resp_body = await resp.read()
-                if self.cfg.log_resp_body:
-                    self._span_annotate_resp_body(span, resp_body, ts2)
-
                 span.tag(HttpSpan.TAG_HTTP_RESPONSE_SIZE, resp.content_length)
                 span.tag(HttpSpan.TAG_HTTP_STATUS_CODE, str(resp.status))
 
+                resp_body = await resp.read()
+
+                if self.cfg.log_resp_body:
+                    self._span_annotate_resp_body(
+                        span,
+                        resp_body,
+                        time.time(),
+                        encoding=resp.charset,
+                    )
+
                 return resp
 
     async def health(self) -> None:
         pass
```

### Comparing `ipapp-1.3.9/ipapp/http/server.py` & `ipapp-2.0.0/ipapp/http/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,32 @@
+import asyncio
 import logging
 import time
 from abc import ABCMeta
 from contextvars import Token
 from datetime import datetime, timezone
 from ssl import SSLContext
-from typing import Awaitable, Callable, Dict, List, Optional, Union
+from typing import (
+    Any,
+    AsyncIterator,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Union,
+)
 
 from aiohttp import web
 from aiohttp.payload import Payload
 from aiohttp.web_log import AccessLogger
 from aiohttp.web_runner import AppRunner, BaseSite, TCPSite
 from aiohttp.web_urldispatcher import AbstractResource, AbstractRoute
+from aiojobs import Scheduler
+from aiojobs.aiohttp import spawn
 from pydantic import BaseModel, Field
 
 import ipapp.app  # noqa
 from ipapp.component import Component
 from ipapp.http._base import HttpSpan
 from ipapp.logger import Span
 from ipapp.misc import (
@@ -36,14 +48,25 @@
 class ServerConfig(BaseModel):
     """
     Конфигурация HTTP сервера
     """
 
     host: str = Field("0.0.0.0", description="Адрес HTTP сервера")  # nosec
     port: int = Field(8080, ge=1, le=65535, description="Порт HTTP сервера")
+    shield: int = Field(
+        False,
+        description="Защищать запросы от отмены перед остановкой сервера",
+    )
+    graceful_timeout: float = Field(
+        60.0,
+        description=(
+            "Максимальное время ожидания завершения запросов "
+            "перед началом остановки сервера"
+        ),
+    )
     shutdown_timeout: float = Field(
         60.0,
         description=(
             "Максимальное время ожидания завершения обработки "
             "входящих запросов перед остановкой сервиса"
         ),
     )
@@ -206,24 +229,41 @@
         self.backlog = cfg.backlog
         self.reuse_address = cfg.reuse_address
         self.reuse_port = cfg.reuse_port
 
         self.sites: List[BaseSite] = []
 
         self.web_app = web.Application()
+        if cfg.shield:
+            self.setup(
+                self.web_app,
+                graceful_timeout=cfg.graceful_timeout,
+                close_timeout=self.shutdown_timeout,
+            )
         self.runner = AppRunner(
             self.web_app,
             handle_signals=True,
             access_log_class=AccessLogger,
             access_log_format=AccessLogger.LOG_FORMAT,
             access_log=access_logger,
         )
-        self.web_app.middlewares.append(self._req_wrapper)
+        self.web_app.middlewares.append(self._middleware)
 
     @web.middleware
+    async def _middleware(
+        self,
+        request: web.Request,
+        handler: Callable[[web.Request], Awaitable[web.StreamResponse]],
+    ) -> Union[web.Response, web.FileResponse]:
+        if self.cfg.shield:
+            job = await spawn(request, self._req_wrapper(request, handler))
+            return await job.wait()
+        else:
+            return await self._req_wrapper(request, handler)
+
     async def _req_wrapper(
         self,
         request: web.Request,
         handler: Callable[[web.Request], Awaitable[web.StreamResponse]],
     ) -> Union[web.Response, web.FileResponse]:
         span_token: Optional[Token] = None
         request_token: Optional[Token] = None
@@ -409,14 +449,35 @@
                 ssl_context=self.ssl_context,
                 backlog=self.backlog,
                 reuse_address=self.reuse_address,
                 reuse_port=self.reuse_port,
             )
         )
 
+    @staticmethod
+    def setup(
+        app: web.Application,
+        graceful_timeout: Optional[float] = None,
+        **kwargs: Any,
+    ) -> None:
+        async def cleanup_context(app: web.Application) -> AsyncIterator[None]:
+            app["AIOJOBS_SCHEDULER"] = scheduler = Scheduler(**kwargs)
+            yield
+            if graceful_timeout and scheduler._jobs:
+                await asyncio.gather(
+                    *[
+                        job.wait(timeout=graceful_timeout)
+                        for job in scheduler._jobs
+                    ],
+                    return_exceptions=True,
+                )
+            await scheduler.close()
+
+        app.cleanup_ctx.append(cleanup_context)
+
     async def start(self) -> None:
         self.app.log_info("Starting HTTP server")
         for site in self.sites:
             await site.start()
 
         names = sorted(str(s.name) for s in self.runner.sites)
         self.app.log_info("Running HTTP server on %s", ', '.join(names))
```

### Comparing `ipapp-1.3.9/ipapp/logger/__init__.py` & `ipapp-2.0.0/ipapp/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/logger/adapters/_abc.py` & `ipapp-2.0.0/ipapp/logger/adapters/_abc.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/logger/adapters/prometheus.py` & `ipapp-2.0.0/ipapp/logger/adapters/prometheus.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/logger/adapters/requests.py` & `ipapp-2.0.0/ipapp/logger/adapters/requests.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/logger/adapters/sentry.py` & `ipapp-2.0.0/ipapp/logger/adapters/sentry.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/logger/adapters/zipkin.py` & `ipapp-2.0.0/ipapp/logger/adapters/zipkin.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/logger/logger.py` & `ipapp-2.0.0/ipapp/logger/logger.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/logger/span.py` & `ipapp-2.0.0/ipapp/logger/span.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/misc.py` & `ipapp-2.0.0/ipapp/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/mq/pika.py` & `ipapp-2.0.0/ipapp/mq/pika.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,15 +529,15 @@
             app=self.amqp.app,
         ) as span:
             span.tag(AmqpSpan.TAG_CHANNEL_NUMBER, str(self._ch.channel_number))
             span.tag(AmqpSpan.TAG_EXCHANGE, str(exchange))
             span.tag(AmqpSpan.TAG_ROUTING_KEY, str(routing_key))
             span.tag(AmqpSpan.TAG_URL, self._conn.pika._masked_url)
 
-            with timeout(self.amqp.cfg.publish_timeout):
+            async with timeout(self.amqp.cfg.publish_timeout):
                 if not self._ch.is_closed or self.name is None:
 
                     if propagate_trace:
                         hdrs = span.to_headers()
                         if properties is None:
                             properties = pika.spec.BasicProperties(
                                 headers=hdrs
```

### Comparing `ipapp-1.3.9/ipapp/openapi/misc.py` & `ipapp-2.0.0/ipapp/openapi/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/openapi/models.py` & `ipapp-2.0.0/ipapp/openapi/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/openapi/templates.py` & `ipapp-2.0.0/ipapp/openapi/templates.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/http/client.py` & `ipapp-2.0.0/ipapp/rpc/http/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/http/server.py` & `ipapp-2.0.0/ipapp/rpc/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/jsonrpc/error.py` & `ipapp-2.0.0/ipapp/rpc/jsonrpc/error.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/jsonrpc/http/client.py` & `ipapp-2.0.0/ipapp/rpc/jsonrpc/http/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/jsonrpc/http/server.py` & `ipapp-2.0.0/ipapp/rpc/jsonrpc/http/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from contextvars import ContextVar
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 
 from aiohttp import web
 from multidict import CIMultiDict
 from pydantic import BaseModel
@@ -46,15 +45,14 @@
     'response_del_cookies', default=[]
 )
 
 
 class JsonRpcHttpHandlerConfig(BaseModel):
     path: str = '/'
     healthcheck_path: str = '/health'
-    shield: bool = False
     discover_enabled: bool = True
     cors_enabled: bool = True
     cors_origin: str = 'https://playground.open-rpc.org'
 
 
 class JsonRpcHttpHandler(_ServerHandler):
     _rpc: JsonRpcExecutor
@@ -77,15 +75,15 @@
             self.app,
             discover_enabled=self._cfg.discover_enabled,
             servers=self._servers,
             external_docs=self._external_docs,
         )
         if self._cfg.healthcheck_path:
             self._setup_healthcheck(self._cfg.healthcheck_path)
-        self.server.add_route('POST', self._cfg.path, self.rpc_handler)
+        self.server.add_route('POST', self._cfg.path, self._handle)
         self.server.add_route(
             'OPTIONS', self._cfg.path, self.rpc_options_handler
         )
         await self._rpc.start_scheduler()
 
     async def stop(self) -> None:
         await self._rpc.stop_scheduler()
@@ -99,20 +97,14 @@
             }
         else:
             return {}
 
     async def rpc_options_handler(self, request: web.Request) -> web.Response:
         return web.HTTPOk(headers=self._get_cors_headers())
 
-    async def rpc_handler(self, request: web.Request) -> web.Response:
-        if self._cfg.shield:
-            return await asyncio.shield(self._handle(request))
-        else:
-            return await self._handle(request)
-
     async def _handle(self, request: web.Request) -> web.Response:
         req_body = await request.read()
         response_set_headers_token = response_set_headers.set(CIMultiDict())
         response_set_cookies_token = response_set_cookies.set([])
         response_del_cookies_token = response_del_cookies.set([])
         resp_body = await self._rpc.exec(req_body)
         resp = web.Response(
```

### Comparing `ipapp-1.3.9/ipapp/rpc/jsonrpc/main.py` & `ipapp-2.0.0/ipapp/rpc/jsonrpc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,15 @@
         self._scheduler: Optional[aiojobs.Scheduler] = None
         self._scheduler_kwargs = scheduler_kwargs or {}
 
         self._servers: Optional[List[Server]] = servers
         self._external_docs: Optional[ExternalDocs] = external_docs
 
     async def start_scheduler(self) -> None:
-        self._scheduler = await aiojobs.create_scheduler(
-            **self._scheduler_kwargs
-        )
+        self._scheduler = aiojobs.Scheduler(**self._scheduler_kwargs)
 
     async def stop_scheduler(self) -> None:
         if self._scheduler is not None:
             await self._scheduler.close()
             self._scheduler = None
 
     async def exec(self, request: bytes) -> bytes:
@@ -391,16 +389,18 @@
             span.tag(SPAN_TAG_JSONRPC_METHOD, method)
         else:
             span.name = 'rpc::in::error'
 
     def _set_span_err(self, err: Exception) -> None:
         if not span:
             return
+        span._exception = err
         span.tag('error', 'true')
         span.annotate(span.ANN_TRACEBACK, traceback.format_exc())
+        span.tag(span.TAG_ERROR_MESSAGE, str(err))
         if hasattr(err, 'jsonrpc_error_code'):
             span.tag(
                 SPAN_TAG_JSONRPC_CODE,
                 str(err.jsonrpc_error_code),  # type: ignore
             )
         else:
             code, _, _ = _get_code_message_and_data(err)
```

### Comparing `ipapp-1.3.9/ipapp/rpc/jsonrpc/mq/pika.py` & `ipapp-2.0.0/ipapp/rpc/jsonrpc/mq/pika.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/discover.py` & `ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/discover.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,16 +309,16 @@
     response = {}
     if ResponseResultModel is not None:
         if getattr(ResponseResultModel, "__name__", "") == response_model_name:
             _fix_model_name(ResponseResultModel, response_result_model_name)
 
         response["result"] = (ResponseResultModel, None)
 
-        ResponseModel: Type[BaseModel] = create_model(
-            response_model_name, **response  # type: ignore
+        ResponseModel: Type[BaseModel] = create_model(  # type: ignore
+            response_model_name, **response
         )
 
         params_def = _get_model_definition(
             ResponseModel, model_name_map, schemas
         )
 
         result_schema = params_def['properties']['result']
```

### Comparing `ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/models.py` & `ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/main.py` & `ipapp-2.0.0/ipapp/rpc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,19 +365,19 @@
             if ispec.kwonlydefaults is None:
                 raise RuntimeError
             self.optional_params[kwargs[i]] = ispec.kwonlydefaults[kwargs[i]]
 
         if len(ispec.annotations) > 0:
             opt = self.optional_params
 
-            self._model = create_model(
+            self._model = create_model(  # type: ignore
                 'Model',
                 __config__=_PydanticConfig,
                 __validators__=validators,
-                **{  # type: ignore
+                **{
                     k: (v, ... if k not in opt else opt[k])
                     for k, v in ispec.annotations.items()
                     if k != 'return' and k != self_name
                 },
             )
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
```

### Comparing `ipapp-1.3.9/ipapp/rpc/mq/pika.py` & `ipapp-2.0.0/ipapp/rpc/mq/pika.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/restrpc/error.py` & `ipapp-2.0.0/ipapp/rpc/restrpc/error.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/restrpc/http/client.py` & `ipapp-2.0.0/ipapp/rpc/restrpc/http/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/rpc/restrpc/http/server.py` & `ipapp-2.0.0/ipapp/rpc/restrpc/http/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import inspect
 import json
 from contextvars import ContextVar
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Callable, Coroutine, Dict, List, Optional, Union
 
@@ -82,15 +81,14 @@
 
 
 class RestRpcHttpHandlerConfig(BaseModel):
     path: str = Field("/", description="Путь Rest-RPC сервера")
     healthcheck_path: str = Field(
         "/health", description="Путь health check RPC сервера"
     )
-    shield: bool = False
     cors_enabled: bool = True
     cors_origin: str = ""
     openapi_json_url: str = Field(
         "/openapi.json", description="Путь публикации OpenAPI спецификации"
     )
     openapi_yaml_url: str = Field(
         "/openapi.yaml", description="Путь публикации OpenAPI спецификации"
@@ -162,19 +160,19 @@
             self.openapi_prepare()
         except Exception as exc:
             self.app.log_err(f"Cannot initialize openapi: {exc}")
         path = self._cfg.path
         if path.endswith("/"):
             path = path[:-1]
         for method_name in self._methods.keys():
-            self.server.add_post(f"{path}/{method_name}/", self.rpc_handler)
+            self.server.add_post(f"{path}/{method_name}/", self._handle)
             self.server.add_options(
                 f"{path}/{method_name}/", self.rpc_options_handler
             )
-            self.server.add_post(f"{path}/{method_name}", self.rpc_handler)
+            self.server.add_post(f"{path}/{method_name}", self._handle)
             self.server.add_options(
                 f"{path}/{method_name}", self.rpc_options_handler
             )
         await self._restrpc.start_scheduler()
 
     async def stop(self) -> None:
         await self._restrpc.stop_scheduler()
@@ -189,19 +187,14 @@
             "Access-Control-Allow-Methods": "OPTIONS, POST",
             "Access-Control-Allow-Headers": "*",
         }
 
     async def rpc_options_handler(self, request: web.Request) -> web.Response:
         return web.HTTPOk(headers=self._get_cors_headers())
 
-    async def rpc_handler(self, request: web.Request) -> web.Response:
-        if self._cfg.shield:
-            return await asyncio.shield(self._handle(request))
-        return await self._handle(request)
-
     async def _handle(self, request: web.Request) -> web.Response:
         req_body = await request.read()
         method_name = request.path
         if method_name.startswith(self._cfg.path):
             method_name = method_name[len(self._cfg.path) :]
         if method_name.startswith("/"):
             method_name = method_name[1:]
```

### Comparing `ipapp-1.3.9/ipapp/rpc/restrpc/main.py` & `ipapp-2.0.0/ipapp/rpc/restrpc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,17 +257,15 @@
             for key in dir(registry):
                 if callable(getattr(registry, key)):
                     fn = getattr(registry, key)
                     if hasattr(fn, '__rpc_name__'):
                         yield fn
 
     async def start_scheduler(self) -> None:
-        self._scheduler = await aiojobs.create_scheduler(
-            **self._scheduler_kwargs
-        )
+        self._scheduler = aiojobs.Scheduler(**self._scheduler_kwargs)
 
     async def stop_scheduler(self) -> None:
         if self._scheduler is None:
             return
         await self._scheduler.close()
         self._scheduler = None
```

### Comparing `ipapp-1.3.9/ipapp/rpc/restrpc/openapi/misc.py` & `ipapp-2.0.0/ipapp/rpc/restrpc/openapi/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/s3/boto.py` & `ipapp-2.0.0/ipapp/s3/boto.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/s3/models.py` & `ipapp-2.0.0/ipapp/s3/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/sftp/client.py` & `ipapp-2.0.0/ipapp/sftp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 import os
 from asyncio import Future
 from enum import Enum
 from pathlib import PurePath
-from typing import Any, Callable, List, Optional, Union, Sequence
+from typing import Any, Callable, List, Optional, Sequence, Union
 
 import asyncssh
 from asyncssh import (
     BytesOrStr,
     SFTPAttrs,
     SFTPClient,
     SFTPName,
```

### Comparing `ipapp-1.3.9/ipapp/sphinx/config.py` & `ipapp-2.0.0/ipapp/sphinx/config.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/task/db.py` & `ipapp-2.0.0/ipapp/task/db.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/utils/lock/local.py` & `ipapp-2.0.0/ipapp/utils/lock/local.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/utils/lock/main.py` & `ipapp-2.0.0/ipapp/utils/lock/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/utils/lock/pg.py` & `ipapp-2.0.0/ipapp/utils/lock/pg.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/ipapp/utils/lock/redis.py` & `ipapp-2.0.0/ipapp/utils/lock/redis.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.9/pyproject.toml` & `ipapp-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   | \.vscode
 )
 '''
 
 [tool.coverage.run]
 branch = true
 source = ["ipapp"]
-omit = ["site-packages", ".tox"]
+omit = ["site-packages"]
 
 [tool.pytest.ini_options]
 addopts = "-s -v --cov --cov-report term --cov-report=html --cov-config pyproject.toml"
 testpaths = ["tests"]
 filterwarnings = ["ignore::DeprecationWarning:distutils"]
 
 [tool.isort]
@@ -28,15 +28,15 @@
 force_grid_wrap = 0
 multi_line_output = 3
 use_parentheses = true
 include_trailing_comma = true
 
 [tool.poetry]
 name = "ipapp"
-version = "1.3.9"
+version = "2.0.0"
 description = "InPlat application framework"
 authors = ["InPlat"]
 classifiers = [
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Intended Audience :: System Administrators',
     'Operating System :: Unix',
@@ -47,18 +47,18 @@
 ]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/inplat/ipapp"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = "^1.8.2"
-aiohttp = "^3.8.1"
+pydantic = "^1.10.2"
+aiohttp = "^3.8.3"
 aiozipkin = ">=0.7,<1.2"
-aiojobs = "^1.0.0"
+aiojobs = "^1.1.0"
 prometheus-client = ">=0.8,<0.12"
 sentry-sdk = "^1.0.0"
 deepmerge = ">=0.2.1,<0.4.0"
 async-timeout = "^4.0.0"
 pyyaml = "^5.4"
 docstring-parser = ">=0.7.1,<0.9.0"
 tinyrpc = "^1.0.4"
@@ -68,49 +68,52 @@
 cx-Oracle = {version = "^8.0.0", optional = true}
 asyncpg = {version = ">=0.22,<0.24", optional = true}
 pika = {version = "^1.2.0", optional = true}
 aiobotocore = {version = "^1.2.2", optional = true}
 python-magic = {version = "^0.4.22", optional = true}
 asyncssh = {version = "^2.3.0", extras = ["pyOpenSSL"], optional = true}
 # testing
-black = {version = "21.9b0", optional = true}
+black = {version = "22.10.0", optional = true}
 flake8 = {version = "3.9.2", optional = true}
 mock = {version = "^4.0.2", optional = true}
-mypy = {version = "0.812", optional = true}
-bandit = {version = "1.6.3", optional = true}
+mypy = {version = "0.982", optional = true}
+bandit = {version = "1.7.2", optional = true}
 isort = {version = "5.9.3", optional = true}
-safety = {version = "^1.10.3", optional = true}
 pylint = {version = "^2.13.4", optional = true}
 pytest-aiohttp = {version = "^0.3.0", optional = true}
 pytest = {version = "^6.1.0", optional = true}
 pytest-asyncio = {version = "^0.14.0", optional = true}
 pytest-cov = {version = "^2.11.0", optional = true}
 coverage = {version = "^5.3", extras = ["toml"], optional = true}
-Sphinx = {version = ">=3.5.2,<5.0.0", optional = true}
-sphinx-rtd-theme = {version = "^0.5.1", optional = true}
-tox = {version = "^3.23.0", optional = true}
+Sphinx = {version = "^5.3.0", optional = true}
+sphinx-rtd-theme = {version = "^1.0.0", optional = true}
 docker-compose = {version = "^1.27.4", optional = true}
 watchdog = {version = "^2.0.2", optional = true}
+pytz = {version = "^2022.7.1", optional = true}
 crontab = {version = ">=0.22.6,<0.24.0", optional = true}
 aioredis = {version = "^1.3.1", optional = true}
+types-docutils = {version = "0.19.1.1", optional = true}
+types-pytz = {version = "^2022.7.1.2", optional = true}
+types-pyyaml = {version = "6.0.12.2", optional = true}
+importlib-metadata = {version = "4.13.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 requests = {version = "^2.25.1", optional = true}
 pytest-httpserver = "^1.0.1"
 autoflake = "^1.4"
 
 [tool.poetry.extras]
 fastapi = ["uvicorn", "fastapi"]
 oracle = ["cx-Oracle"]
 postgres = ["asyncpg"]
 redis = ["aioredis"]
 rabbitmq = ["pika"]
 s3 = ["aiobotocore", "python-magic"]
 sftp = ["asyncssh"]
-dbtm = ["asyncpg", "crontab"]
-testing = ["black", "flake8", "mock", "mypy", "bandit", "isort", "safety", "pylint", "pytest-aiohttp", "pytest",
-    "pytest-asyncio", "pytest-cov", "coverage", "Sphinx", "sphinx-rtd-theme", "pip", "wheel", "tox",
-    "docker-compose", "watchdog"]
+dbtm = ["asyncpg", "crontab", "pytz"]
+testing = ["black", "flake8", "mock", "mypy", "bandit", "isort", "pylint", "pytest-aiohttp", "pytest",
+    "pytest-asyncio", "pytest-cov", "coverage", "Sphinx", "sphinx-rtd-theme", "types-docutils", "types-pytz",
+    "docker-compose", "watchdog", "types-pyyaml", "importlib-metadata"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ipapp-1.3.9/PKG-INFO` & `ipapp-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 Metadata-Version: 2.1
 Name: ipapp
-Version: 1.3.9
+Version: 2.0.0
 Summary: InPlat application framework
 Home-page: https://github.com/inplat/ipapp
 License: MIT
 Author: InPlat
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dbtm
 Provides-Extra: fastapi
 Provides-Extra: oracle
 Provides-Extra: postgres
 Provides-Extra: rabbitmq
 Provides-Extra: redis
 Provides-Extra: s3
 Provides-Extra: sftp
 Provides-Extra: testing
-Requires-Dist: Sphinx (>=3.5.2,<5.0.0); extra == "testing"
-Requires-Dist: aiobotocore (>=1.2.2,<2.0.0); extra == "s3"
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: aiojobs (>=1.0.0,<2.0.0)
-Requires-Dist: aioredis (>=1.3.1,<2.0.0); extra == "redis"
+Requires-Dist: Sphinx (>=5.3.0,<6.0.0) ; extra == "testing"
+Requires-Dist: aiobotocore (>=1.2.2,<2.0.0) ; extra == "s3"
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: aiojobs (>=1.1.0,<2.0.0)
+Requires-Dist: aioredis (>=1.3.1,<2.0.0) ; extra == "redis"
 Requires-Dist: aiozipkin (>=0.7,<1.2)
 Requires-Dist: async-timeout (>=4.0.0,<5.0.0)
-Requires-Dist: asyncpg (>=0.22,<0.24); extra == "postgres" or extra == "dbtm"
-Requires-Dist: asyncssh[pyOpenSSL] (>=2.3.0,<3.0.0); extra == "sftp"
-Requires-Dist: bandit (==1.6.3); extra == "testing"
-Requires-Dist: black (==21.9b0); extra == "testing"
-Requires-Dist: coverage[toml] (>=5.3,<6.0); extra == "testing"
-Requires-Dist: crontab (>=0.22.6,<0.24.0); extra == "dbtm"
-Requires-Dist: cx-Oracle (>=8.0.0,<9.0.0); extra == "oracle"
+Requires-Dist: asyncpg (>=0.22,<0.24) ; extra == "postgres" or extra == "dbtm"
+Requires-Dist: asyncssh[pyopenssl] (>=2.3.0,<3.0.0) ; extra == "sftp"
+Requires-Dist: bandit (==1.7.2) ; extra == "testing"
+Requires-Dist: black (==22.10.0) ; extra == "testing"
+Requires-Dist: coverage[toml] (>=5.3,<6.0) ; extra == "testing"
+Requires-Dist: crontab (>=0.22.6,<0.24.0) ; extra == "dbtm"
+Requires-Dist: cx-Oracle (>=8.0.0,<9.0.0) ; extra == "oracle"
 Requires-Dist: deepmerge (>=0.2.1,<0.4.0)
-Requires-Dist: docker-compose (>=1.27.4,<2.0.0); extra == "testing"
+Requires-Dist: docker-compose (>=1.27.4,<2.0.0) ; extra == "testing"
 Requires-Dist: docstring-parser (>=0.7.1,<0.9.0)
-Requires-Dist: fastapi (>=0.75.2,<0.76.0); extra == "fastapi"
-Requires-Dist: flake8 (==3.9.2); extra == "testing"
-Requires-Dist: isort (==5.9.3); extra == "testing"
+Requires-Dist: fastapi (>=0.75.2,<0.76.0) ; extra == "fastapi"
+Requires-Dist: flake8 (==3.9.2) ; extra == "testing"
+Requires-Dist: importlib-metadata (==4.13.0) ; extra == "testing"
+Requires-Dist: isort (==5.9.3) ; extra == "testing"
 Requires-Dist: jsonschema (>=3.2.0,<4.0.0)
-Requires-Dist: mock (>=4.0.2,<5.0.0); extra == "testing"
-Requires-Dist: mypy (==0.812); extra == "testing"
-Requires-Dist: pika (>=1.2.0,<2.0.0); extra == "rabbitmq"
+Requires-Dist: mock (>=4.0.2,<5.0.0) ; extra == "testing"
+Requires-Dist: mypy (==0.982) ; extra == "testing"
+Requires-Dist: pika (>=1.2.0,<2.0.0) ; extra == "rabbitmq"
 Requires-Dist: prometheus-client (>=0.8,<0.12)
-Requires-Dist: pydantic (>=1.8.2,<2.0.0)
-Requires-Dist: pylint (>=2.13.4,<3.0.0); extra == "testing"
-Requires-Dist: pytest (>=6.1.0,<7.0.0); extra == "testing"
-Requires-Dist: pytest-aiohttp (>=0.3.0,<0.4.0); extra == "testing"
-Requires-Dist: pytest-asyncio (>=0.14.0,<0.15.0); extra == "testing"
-Requires-Dist: pytest-cov (>=2.11.0,<3.0.0); extra == "testing"
-Requires-Dist: python-magic (>=0.4.22,<0.5.0); extra == "s3"
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pylint (>=2.13.4,<3.0.0) ; extra == "testing"
+Requires-Dist: pytest (>=6.1.0,<7.0.0) ; extra == "testing"
+Requires-Dist: pytest-aiohttp (>=0.3.0,<0.4.0) ; extra == "testing"
+Requires-Dist: pytest-asyncio (>=0.14.0,<0.15.0) ; extra == "testing"
+Requires-Dist: pytest-cov (>=2.11.0,<3.0.0) ; extra == "testing"
+Requires-Dist: python-magic (>=0.4.22,<0.5.0) ; extra == "s3"
+Requires-Dist: pytz (>=2022.7.1,<2023.0.0) ; extra == "dbtm"
 Requires-Dist: pyyaml (>=5.4,<6.0)
-Requires-Dist: safety (>=1.10.3,<2.0.0); extra == "testing"
 Requires-Dist: sentry-sdk (>=1.0.0,<2.0.0)
-Requires-Dist: sphinx-rtd-theme (>=0.5.1,<0.6.0); extra == "testing"
+Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "testing"
 Requires-Dist: tinyrpc (>=1.0.4,<2.0.0)
-Requires-Dist: tox (>=3.23.0,<4.0.0); extra == "testing"
-Requires-Dist: uvicorn (>=0.12.1,<0.16.0); extra == "fastapi"
-Requires-Dist: watchdog (>=2.0.2,<3.0.0); extra == "testing"
+Requires-Dist: types-docutils (==0.19.1.1) ; extra == "testing"
+Requires-Dist: types-pytz (>=2022.7.1.2,<2023.0.0.0) ; extra == "testing"
+Requires-Dist: types-pyyaml (==6.0.12.2) ; extra == "testing"
+Requires-Dist: uvicorn (>=0.12.1,<0.16.0) ; extra == "fastapi"
+Requires-Dist: watchdog (>=2.0.2,<3.0.0) ; extra == "testing"
 Description-Content-Type: text/markdown
 
 # InPlat application framework
 > Framework with asyncio based on python.
 
 ![PyPI](https://img.shields.io/pypi/v/ipapp?style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ipapp?style=for-the-badge) ![Read the Docs](https://img.shields.io/readthedocs/ipapp?style=for-the-badge)
```

