# Comparing `tmp/ralph-malph-3.6.0.tar.gz` & `tmp/ralph-malph-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralph-malph-3.6.0.tar", last modified: Wed May 17 11:54:32 2023, max compression
+gzip compressed data, was "ralph-malph-3.7.0.tar", last modified: Tue Jun 13 16:36:04 2023, max compression
```

## Comparing `ralph-malph-3.6.0.tar` & `ralph-malph-3.7.0.tar`

### file list

```diff
@@ -1,145 +1,176 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.576460 ralph-malph-3.6.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6443 2023-05-17 11:54:32.576460 ralph-malph-3.6.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5291 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2655 2023-05-17 11:54:32.576460 ralph-malph-3.6.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.560460 ralph-malph-3.6.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.560460 ralph-malph-3.6.0/src/ralph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.560460 ralph-malph-3.6.0/src/ralph/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1406 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5321 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/auth.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/forwarding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1573 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/api/routers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/routers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/routers/health.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15226 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/routers/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/backends/database/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3688 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/base.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    12909 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8536 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/mixins.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/backends/storage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/ldp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5171 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/swift.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/backends/stream/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/stream/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/stream/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/stream/ws.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19679 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10326 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/converter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/models/edx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/browser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/models/edx/converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/navigational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7162 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/navigational/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/navigational/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/navigational/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/navigational/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/navigational/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/navigational/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/video/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/video/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/selector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      356 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1820 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3802 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/actors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/attachments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2380 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1941 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3941 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/unnested_objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1554 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/verbs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1201 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1304 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8241 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5335 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/verbs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7490 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph_malph.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6443 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4104 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.576460 ralph-malph-3.6.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3521 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_auth.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9427 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_cli_usage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_dependencies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5291 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.348669 ralph-malph-3.7.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/api/auth/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/auth/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5871 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/auth/basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4882 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/auth/oidc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/auth/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/forwarding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/api/routers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/routers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/routers/health.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16304 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/routers/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/backends/database/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/base.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13603 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9315 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9873 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/mongo.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/backends/http/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/http/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3713 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/http/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10463 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/http/lrs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/mixins.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/backends/storage/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/ldp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5310 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/swift.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/backends/stream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/stream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/stream/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/stream/ws.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21725 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12019 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/edx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/browser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/edx/converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3000 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/navigational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7195 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/navigational/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/navigational/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/navigational/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/navigational/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/navigational/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/navigational/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/video/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/video/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/selector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2055 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/attachments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2411 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/ifi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1455 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3067 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4079 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/unnested_objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/verbs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      900 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      703 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4575 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/navigation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/navigation/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/navigation/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8686 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/video/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5263 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/video/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6947 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/video/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7328 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12787 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/src/ralph_malph.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5465 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9942 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_cli_usage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_dependencies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_utils.py
```

### Comparing `ralph-malph-3.6.0/LICENSE.md` & `ralph-malph-3.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/PKG-INFO` & `ralph-malph-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.6.0
+Version: 3.7.0
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: backend-clickhouse
 Provides-Extra: backend-es
 Provides-Extra: backend-ldp
+Provides-Extra: backend-lrs
 Provides-Extra: backend-mongo
 Provides-Extra: backend-s3
 Provides-Extra: backend-swift
 Provides-Extra: backend-ws
 Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: ci
```

### Comparing `ralph-malph-3.6.0/README.md` & `ralph-malph-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/setup.cfg` & `ralph-malph-3.7.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ralph-malph
-version = 3.6.0
+version = 3.7.0
 description = The ultimate toolbox for your learning analytics
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://openfun.github.io/ralph/
 license = MIT
@@ -38,14 +38,17 @@
 	clickhouse-connect[numpy,pandas]<0.6
 	python-dateutil>=2.8.2
 backend-es = 
 	elasticsearch>=8.0.0
 backend-ldp = 
 	ovh>=1.0.0
 	requests>=2.0.0
+backend-lrs = 
+	httpx==0.24.1
+	more-itertools==9.1.0
 backend-mongo = 
 	pymongo[srv]>=4.0.0
 	python-dateutil>=2.8.2
 backend-s3 = 
 	boto3>=1.24.70
 	botocore>=1.27.71
 backend-swift = 
@@ -57,38 +60,43 @@
 	bcrypt>=4.0.0
 	click>=8.1.0
 	click-option-group>=0.5.0
 	sentry-sdk[fastapi]>=1.9.0
 dev = 
 	bandit==1.7.5
 	black==23.3.0
+	cryptography==40.0.1
 	factory-boy==3.2.1
 	flake8==6.0.0
-	hypothesis==6.75.3
+	hypothesis==6.78.1
 	isort==5.12.0
 	logging-gelf==0.0.26
 	mkdocs==1.4.3
 	mkdocs-click==0.8.0
-	mkdocs-material==9.1.12
-	mkdocstrings[python-legacy]==0.21.2
-	moto==4.1.9
+	mkdocs-material==9.1.15
+	mkdocstrings[python-legacy]==0.22.0
+	moto==4.1.11
 	pydocstyle==6.3.0
 	pyfakefs==5.2.2
 	pylint==2.17.4
-	pytest==7.3.1
+	pytest==7.3.2
 	pytest-asyncio==0.21.0
-	pytest-cov==4.0.0
+	pytest-cov==4.1.0
+	pytest-httpx==0.22.0
+	responses==0.23.1
 ci = 
 	twine==4.0.2
 lrs = 
 	bcrypt==4.0.1
-	fastapi==0.95.1
+	fastapi==0.97.0
+	cachetools==5.3.1
 	h11>=0.11.0
-	httpx==0.24.0
-	sentry_sdk==1.22.2
+	httpx==0.24.1
+	sentry_sdk==1.25.1
+	python-jose==3.3.0
 	uvicorn[standard]==0.22.0
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
@@ -117,15 +125,15 @@
 [isort]
 known_ralph = ralph
 sections = FUTURE,STDLIB,THIRDPARTY,RALPH,FIRSTPARTY,LOCALFOLDER
 skip_glob = venv
 profile = black
 
 [tool:pytest]
-addopts = -v --cov-report term-missing --cov-config=.coveragerc --cov=src/ralph
+addopts = -v --cov-report term-missing --cov-config=.coveragerc --cov=ralph
 python_files = 
 	test_*.py
 	tests.py
 testpaths = 
 	tests
 
 [egg_info]
```

### Comparing `ralph-malph-3.6.0/src/ralph/__main__.py` & `ralph-malph-3.7.0/src/ralph/__main__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/api/__init__.py` & `ralph-malph-3.7.0/src/ralph/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import sentry_sdk
 from fastapi import Depends, FastAPI
 
 from ralph.conf import settings
 
 from .. import __version__
-from .auth import AuthenticatedUser, authenticated_user
+from .auth import get_authenticated_user
+from .auth.user import AuthenticatedUser
 from .routers import health, statements
 
 
 @lru_cache(maxsize=None)
 def get_health_check_routes():
     """Return the health check routes."""
     return [route.path for route in health.router.routes]
@@ -40,10 +41,12 @@
 
 app = FastAPI()
 app.include_router(statements.router)
 app.include_router(health.router)
 
 
 @app.get("/whoami")
-async def whoami(user: AuthenticatedUser = Depends(authenticated_user)):
+async def whoami(
+    user: AuthenticatedUser = Depends(get_authenticated_user),
+):
     """Return the current user's username along with their scopes."""
     return {"username": user.username, "scopes": user.scopes}
```

### Comparing `ralph-malph-3.6.0/src/ralph/api/auth.py` & `ralph-malph-3.7.0/src/ralph/api/auth/basic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,37 @@
-"""Authentication & authorization related tools for the Ralph API."""
+"""Basic authentication & authorization related tools for the Ralph API."""
 
 import logging
 from functools import lru_cache
 from pathlib import Path
-from typing import List
+from threading import Lock
+from typing import List, Union
 
 import bcrypt
+from cachetools import TTLCache, cached
 from fastapi import Depends, HTTPException, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from pydantic import BaseModel, root_validator
 from starlette.authentication import AuthenticationError
 
+from ralph.api.auth.user import AuthenticatedUser
 from ralph.conf import settings
 
 # Unused password used to avoid timing attacks, by comparing passwords supplied
 # with invalid credentials to something innocuous with the same method as if
 # it were a legitimate user.
 UNUSED_PASSWORD = bcrypt.hashpw(b"ralph", bcrypt.gensalt())
 
 
-security = HTTPBasic()
+security = HTTPBasic(auto_error=False)
 
 # API auth logger
 logger = logging.getLogger(__name__)
 
 
-class AuthenticatedUser(BaseModel):
-    """Pydantic model for user authentication.
-
-    Attributes:
-        username (str): Consists of the username of the current user.
-        scopes (List): Consists of the scopes the user has access to.
-    """
-
-    username: str
-    scopes: List[str]
-
-
 class UserCredentials(AuthenticatedUser):
     """Pydantic model for user credentials as stored in the credentials file.
 
     Attributes:
         username (str): Consists of the username for a declared user.
         hash (str): Consists of the hashed password for a declared user.
         scopes (List): Consists of the scopes a declared has access to.
@@ -104,24 +95,50 @@
     if not auth_file.exists():
         msg = "Credentials file <%s> not found."
         logger.warning(msg, auth_file)
         raise AuthenticationError(msg.format(auth_file))
     return ServerUsersCredentials.parse_file(auth_file)
 
 
-def authenticated_user(credentials: HTTPBasicCredentials = Depends(security)):
+@cached(
+    TTLCache(maxsize=settings.AUTH_CACHE_MAX_SIZE, ttl=settings.AUTH_CACHE_TTL),
+    lock=Lock(),
+    key=lambda credentials: (
+        credentials.username,
+        credentials.password,
+    )
+    if credentials is not None
+    else None,
+)
+def get_authenticated_user(
+    credentials: Union[HTTPBasicCredentials, None] = Depends(security),
+) -> AuthenticatedUser:
     """Checks valid auth parameters.
 
     Gets the basic auth parameters from the Authorization header, and checks them
     against our own list of hashed credentials.
 
     Args:
         credentials (iterator): auth parameters from the Authorization header
 
+    Return:
+        AuthenticatedUser (AuthenticatedUser)
+
+    Raises:
+        HTTPException
+
     """
+    if not credentials:
+        logger.error("The basic authentication mode requires a Basic Auth header")
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Could not validate credentials",
+            headers={"WWW-Authenticate": "Basic"},
+        )
+
     try:
         user = next(
             filter(
                 lambda u: u.username == credentials.username,
                 get_stored_credentials(settings.AUTH_FILE),
             )
         )
```

### Comparing `ralph-malph-3.6.0/src/ralph/api/forwarding.py` & `ralph-malph-3.7.0/src/ralph/api/forwarding.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/api/models.py` & `ralph-malph-3.7.0/src/ralph/api/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """API-specific data models definition.
 
 Allows to be exactly as lax as we want when it comes to exact object shape and
 validation.
 """
-from typing import Optional
+from typing import Optional, Union
 from uuid import UUID
 
 from pydantic import AnyUrl, BaseModel, Extra
 
-from ..models.xapi.fields.actors import ActorField
+from ..models.xapi.base.agents import BaseXapiAgent
+from ..models.xapi.base.groups import BaseXapiGroup
 
 
 class ErrorDetail(BaseModel):
     """Pydantic model for errors raised detail.
 
     Type for return value for errors raised in API endpoints.
     Useful for OpenAPI documentation generation.
@@ -58,11 +59,11 @@
 class LaxStatement(BaseModelWithLaxConfig):
     """Pydantic model for lax statement.
 
     It accepts without validating all fields beyond the bare minimum required to
     qualify an object as an XAPI statement.
     """
 
-    actor: ActorField
+    actor: Union[BaseXapiAgent, BaseXapiGroup]
     id: Optional[UUID]
     object: LaxObjectField
     verb: LaxVerbField
```

### Comparing `ralph-malph-3.6.0/src/ralph/api/routers/health.py` & `ralph-malph-3.7.0/src/ralph/api/routers/health.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/api/routers/statements.py` & `ralph-malph-3.7.0/src/ralph/api/routers/statements.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,37 @@
     BackgroundTasks,
     Depends,
     HTTPException,
     Query,
     Request,
     status,
 )
+from pydantic import parse_raw_as
+from pydantic.types import Json
 
+from ralph.api.auth import get_authenticated_user
 from ralph.api.forwarding import forward_xapi_statements, get_active_xapi_forwardings
 from ralph.backends.database.base import BaseDatabase, StatementParameters
 from ralph.conf import settings
 from ralph.exceptions import BackendException, BadFormatException
+from ralph.models.xapi.base.agents import (
+    BaseXapiAgent,
+    BaseXapiAgentWithAccount,
+    BaseXapiAgentWithMbox,
+    BaseXapiAgentWithMboxSha1Sum,
+    BaseXapiAgentWithOpenId,
+)
 
-from ..auth import authenticated_user
 from ..models import ErrorDetail, LaxStatement
 
 logger = logging.getLogger(__name__)
 
 router = APIRouter(
     prefix="/xAPI/statements",
-    dependencies=[Depends(authenticated_user)],
+    dependencies=[Depends(get_authenticated_user)],
 )
 
 
 DATABASE_CLIENT: BaseDatabase = getattr(
     settings.BACKENDS.DATABASE, settings.RUNSERVER_BACKEND.upper()
 ).get_instance()
 
@@ -58,16 +67,15 @@
     ###
     # pylint: disable=invalid-name
     statementId: Optional[str] = Query(None, description="Id of Statement to fetch"),
     # pylint: disable=invalid-name, unused-argument
     voidedStatementId: Optional[str] = Query(
         None, description="**Not implemented** Id of voided Statement to fetch"
     ),
-    # NB: ActorField, which is the specific type expected, is not valid as a query param
-    agent: Optional[str] = Query(
+    agent: Optional[Json] = Query(
         None,
         description=(
             "Filter, only return Statements for which the specified "
             "Agent or Group is the Actor or Object of the Statement"
         ),
     ),
     verb: Optional[str] = Query(
@@ -224,18 +232,36 @@
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=(
                 "Querying by id only accepts `attachments` and `format` as extra"
                 "parameters"
             ),
         )
 
+    # Parse the agent parameter (JSON) into multiple string parameters
+    query_params = dict(request.query_params)
+    if query_params.get("agent") is not None:
+        # Transform agent to `dict` as FastAPI cannot parse JSON (seen as string)
+        agent = parse_raw_as(BaseXapiAgent, query_params["agent"])
+
+        query_params.pop("agent")
+
+        if isinstance(agent, BaseXapiAgentWithMbox):
+            query_params["agent__mbox"] = agent.mbox
+        elif isinstance(agent, BaseXapiAgentWithMboxSha1Sum):
+            query_params["agent__mbox_sha1sum"] = agent.mbox_sha1sum
+        elif isinstance(agent, BaseXapiAgentWithOpenId):
+            query_params["agent__openid"] = agent.openid
+        elif isinstance(agent, BaseXapiAgentWithAccount):
+            query_params["agent__account__name"] = agent.account.name
+            query_params["agent__account__home_page"] = agent.account.homePage
+
     # Query Database
     try:
         query_result = DATABASE_CLIENT.query_statements(
-            StatementParameters(**{**request.query_params, "limit": limit})
+            StatementParameters(**{**query_params, "limit": limit})
         )
     except BackendException as error:
         raise HTTPException(
             status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
             detail="xAPI statements query failed",
         ) from error
```

### Comparing `ralph-malph-3.6.0/src/ralph/backends/database/base.py` & `ralph-malph-3.7.0/src/ralph/backends/database/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,29 +47,60 @@
 class StatementParameters:
     """Represents a dictionary of possible LRS query parameters."""
 
     # pylint: disable=too-many-instance-attributes
 
     statementId: Optional[str] = None  # pylint: disable=invalid-name
     voidedStatementId: Optional[str] = None  # pylint: disable=invalid-name
-    agent: Optional[str] = None
+    agent__mbox: Optional[str] = None
+    agent__mbox_sha1sum: Optional[str] = None
+    agent__openid: Optional[str] = None
+    agent__account__name: Optional[str] = None
+    agent__account__home_page: Optional[str] = None
     verb: Optional[str] = None
     activity: Optional[str] = None
     registration: Optional[UUID] = None
     related_activities: Optional[bool] = False
     related_agents: Optional[bool] = False
     since: Optional[datetime] = None
     until: Optional[datetime] = None
     limit: Optional[int] = None
     format: Optional[Literal["ids", "exact", "canonical"]] = "exact"
     attachments: Optional[bool] = False
     ascending: Optional[bool] = False
     search_after: Optional[str] = None
     pit_id: Optional[str] = None
 
+    def __post_init__(self):
+        """Perform additional conformity verifications on parameters."""
+        # Check that both `homePage` and `name` are provided if `account` is being used
+        if (self.agent__account__name is not None) != (
+            self.agent__account__home_page is not None
+        ):
+            raise BackendParameterException(
+                "Invalid agent parameters: home_page and name are both required"
+            )
+
+        # Check that no more than one Inverse Functional Identifier is provided
+        if (
+            sum(
+                x is not None
+                for x in [
+                    self.agent__mbox,
+                    self.agent__mbox_sha1sum,
+                    self.agent__openid,
+                    self.agent__account__name,
+                ]
+            )
+            > 1
+        ):
+            raise BackendParameterException(
+                "Invalid agent parameters: Only one identifier can be used"
+            )
+
 
 def enforce_query_checks(method):
     """Enforce query argument type checking for methods using it."""
 
     @functools.wraps(method)
     def wrapper(*args, **kwargs):
         """Wrap method execution."""
```

### Comparing `ralph-malph-3.6.0/src/ralph/backends/database/clickhouse.py` & `ralph-malph-3.7.0/src/ralph/backends/database/clickhouse.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses import asdict
 from typing import Generator, List, Optional, TextIO, Union
 
 import clickhouse_connect
 from clickhouse_connect.driver.exceptions import ClickHouseError
 from pydantic import BaseModel, ValidationError
 
-from ralph.conf import settings
+from ralph.conf import ClickhouseClientOptions, settings
 from ralph.exceptions import BackendException, BadFormatException
 
 from .base import (
     BaseDatabase,
     BaseQuery,
     DatabaseStatus,
     StatementParameters,
@@ -50,15 +50,15 @@
         self,
         host: str = clickhouse_settings.HOST,
         port: int = clickhouse_settings.PORT,
         database: str = clickhouse_settings.DATABASE,
         event_table_name: str = clickhouse_settings.EVENT_TABLE_NAME,
         username: str = clickhouse_settings.USERNAME,
         password: str = clickhouse_settings.PASSWORD,
-        client_options: dict = clickhouse_settings.CLIENT_OPTIONS,
+        client_options: ClickhouseClientOptions = clickhouse_settings.CLIENT_OPTIONS,
     ):
         """Instantiates the ClickHouse configuration.
 
         Args:
             host (str): ClickHouse server host to connect to.
             port (int): ClickHouse server port to connect to.
             database (str): ClickHouse database to connect to.
@@ -72,14 +72,16 @@
         user "default".
         """
         if client_options is None:
             client_options = {
                 "date_time_input_format": "best_effort",  # Allows RFC dates
                 "allow_experimental_object_type": 1,  # Allows JSON data type
             }
+        else:
+            client_options = client_options.dict()
 
         self.host = host
         self.port = port
         self.database = database
         self.event_table_name = event_table_name
         self.username = username
         self.password = password
@@ -273,16 +275,32 @@
         """Returns the results of a statements query using xAPI parameters."""
         params = asdict(params)
         where_clauses = []
 
         if params["statementId"]:
             where_clauses.append("event_id = {statementId:UUID}")
 
-        if params["agent"]:
-            where_clauses.append("event.actor.account.name = {agent:String}")
+        if params["agent__mbox"]:
+            where_clauses.append("event.actor.mbox = {agent__mbox:String}")
+
+        if params["agent__mbox_sha1sum"]:
+            where_clauses.append(
+                "event.actor.mbox_sha1sum = {agent__mbox_sha1sum:String}"
+            )
+
+        if params["agent__openid"]:
+            where_clauses.append("event.actor.openid = {agent__openid:String}")
+
+        if params["agent__account__name"]:
+            where_clauses.append(
+                "event.actor.account.name = {agent__account__name:String}"
+            )
+            where_clauses.append(
+                "event.actor.account.homePage = {agent__account__home_page:String}"
+            )
 
         if params["verb"]:
             where_clauses.append("event.verb.id = {verb:String}")
 
         if params["activity"]:
             where_clauses.append("event.object.objectType = 'Activity'")
             where_clauses.append("event.object.id = {activity:String}")
```

### Comparing `ralph-malph-3.6.0/src/ralph/backends/database/es.py` & `ralph-malph-3.7.0/src/ralph/backends/database/es.py`

 * *Files 8% similar despite different names*

```diff
@@ -144,21 +144,43 @@
             raise BackendException(
                 *error.args, f"{documents} succeeded writes"
             ) from error
         return documents
 
     def query_statements(self, params: StatementParameters) -> StatementQueryResult:
         """Returns the results of a statements query using xAPI parameters."""
+        # pylint: disable=too-many-branches
+
         es_query_filters = []
 
         if params.statementId:
             es_query_filters += [{"term": {"_id": params.statementId}}]
 
-        if params.agent:
-            es_query_filters += [{"term": {"actor.account.name.keyword": params.agent}}]
+        if params.agent__mbox:
+            es_query_filters += [{"term": {"actor.mbox.keyword": params.agent__mbox}}]
+
+        if params.agent__mbox_sha1sum:
+            es_query_filters += [
+                {"term": {"actor.mbox_sha1sum.keyword": params.agent__mbox_sha1sum}}
+            ]
+
+        if params.agent__openid:
+            es_query_filters += [
+                {"term": {"actor.openid.keyword": params.agent__openid}}
+            ]
+
+        if params.agent__account__name:
+            es_query_filters += [
+                {"term": {"actor.account.name.keyword": params.agent__account__name}},
+                {
+                    "term": {
+                        "actor.account.homePage.keyword": params.agent__account__home_page  # pylint: disable=line-too-long # noqa: E501
+                    }
+                },
+            ]
 
         if params.verb:
             es_query_filters += [{"term": {"verb.id.keyword": params.verb}}]
 
         if params.activity:
             es_query_filters += [
                 {"term": {"object.objectType.keyword": "Activity"}},
```

### Comparing `ralph-malph-3.6.0/src/ralph/backends/database/mongo.py` & `ralph-malph-3.7.0/src/ralph/backends/database/mongo.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,16 +188,32 @@
     def query_statements(self, params: StatementParameters) -> StatementQueryResult:
         """Returns the results of a statements query using xAPI parameters."""
         mongo_query_filters = {}
 
         if params.statementId:
             mongo_query_filters.update({"_source.id": params.statementId})
 
-        if params.agent:
-            mongo_query_filters.update({"_source.actor.account.name": params.agent})
+        if params.agent__mbox:
+            mongo_query_filters.update({"_source.actor.mbox": params.agent__mbox})
+
+        if params.agent__mbox_sha1sum:
+            mongo_query_filters.update(
+                {"_source.actor.mbox_sha1sum": params.agent__mbox_sha1sum}
+            )
+
+        if params.agent__openid:
+            mongo_query_filters.update({"_source.actor.openid": params.agent__openid})
+
+        if params.agent__account__name:
+            mongo_query_filters.update(
+                {"_source.actor.account.name": params.agent__account__name}
+            )
+            mongo_query_filters.update(
+                {"_source.actor.account.homePage": params.agent__account__home_page}
+            )
 
         if params.verb:
             mongo_query_filters.update({"_source.verb.id": params.verb})
 
         if params.activity:
             mongo_query_filters.update(
                 {
```

### Comparing `ralph-malph-3.6.0/src/ralph/backends/mixins.py` & `ralph-malph-3.7.0/src/ralph/backends/mixins.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/backends/storage/base.py` & `ralph-malph-3.7.0/src/ralph/backends/storage/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/backends/storage/fs.py` & `ralph-malph-3.7.0/src/ralph/backends/storage/fs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/backends/storage/ldp.py` & `ralph-malph-3.7.0/src/ralph/backends/storage/ldp.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/backends/storage/s3.py` & `ralph-malph-3.7.0/src/ralph/backends/storage/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,28 +28,31 @@
     def __init__(
         self,
         access_key_id: str = s3_settings.ACCESS_KEY_ID,
         secret_access_key: str = s3_settings.SECRET_ACCESS_KEY,
         session_token: str = s3_settings.SESSION_TOKEN,
         default_region: str = s3_settings.DEFAULT_REGION,
         bucket_name: str = s3_settings.BUCKET_NAME,
+        endpoint_url: str = s3_settings.ENDPOINT_URL,
     ):
         """Instantiates the AWS S3 client."""
         self.access_key_id = access_key_id
         self.secret_access_key = secret_access_key
         self.session_token = session_token
         self.default_region = default_region
         self.bucket_name = bucket_name
+        self.endpoint_url = endpoint_url
 
         self.client = boto3.client(
             "s3",
             aws_access_key_id=self.access_key_id,
             aws_secret_access_key=self.secret_access_key,
             aws_session_token=self.session_token,
             region_name=self.default_region,
+            endpoint_url=self.endpoint_url,
         )
 
         # Check whether bucket exists and is accessible
         try:
             self.client.head_bucket(Bucket=self.bucket_name)
         except ClientError as err:
             error_msg = err.response["Error"]["Message"]
```

### Comparing `ralph-malph-3.6.0/src/ralph/backends/storage/swift.py` & `ralph-malph-3.7.0/src/ralph/backends/storage/swift.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/backends/stream/ws.py` & `ralph-malph-3.7.0/src/ralph/backends/stream/ws.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/cli.py` & `ralph-malph-3.7.0/src/ralph/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # use all commands except the runserver command when lrs optional
     # dependencies are not installed.
     pass
 from click_option_group import optgroup
 from pydantic import BaseModel
 
 from ralph import __version__ as ralph_version
-from ralph.conf import ClientOptions, CommaSeparatedTuple, settings
+from ralph.conf import ClientOptions, CommaSeparatedTuple, HeadersParameters, settings
 from ralph.exceptions import UnsupportedBackendException
 from ralph.logger import configure_logging
 from ralph.models.converter import Converter
 from ralph.models.selector import ModelSelector
 from ralph.models.validator import Validator
 from ralph.utils import (
     get_backend_instance,
@@ -126,14 +126,36 @@
         """
         if isinstance(value, self.client_options_type):
             return value
 
         return self.client_options_type(**super().convert(value, param, ctx))
 
 
+class HeadersParametersParamType(CommaSeparatedKeyValueParamType):
+    """Comma separated key=value parameter type for headers parameters."""
+
+    def __init__(self, headers_parameters_type):
+        """Instantiates HeadersParametersParamType for a headers_parameters_type.
+
+        Args:
+            headers_parameters_type (any): Pydantic model used for headers parameters.
+        """
+        self.headers_parameters_type = headers_parameters_type
+
+    def convert(self, value, param, ctx):
+        """Splits the values by comma and equal sign.
+
+        Returns an instance of headers_parameters_type build with key/value pairs.
+        """
+        if isinstance(value, self.headers_parameters_type):
+            return value
+
+        return self.headers_parameters_type(**super().convert(value, param, ctx))
+
+
 class JSONStringParamType(click.ParamType):
     """JSON string parameter type."""
 
     name = '\'{"key": "value", "key": "value"}\''
 
     def convert(self, value, param, ctx):
         """Load value as a json string and return a dict."""
@@ -188,14 +210,18 @@
                         option_kwargs["is_flag"] = True
                     elif field_type is dict:
                         option_kwargs["type"] = CommaSeparatedKeyValueParamType()
                     elif field_type is CommaSeparatedTuple:
                         option_kwargs["type"] = CommaSeparatedTupleParamType()
                     elif isclass(field_type) and issubclass(field_type, ClientOptions):
                         option_kwargs["type"] = ClientOptionsParamType(field_type)
+                    elif isclass(field_type) and issubclass(
+                        field_type, HeadersParameters
+                    ):
+                        option_kwargs["type"] = HeadersParametersParamType(field_type)
 
                     command = optgroup.option(
                         option.lower(), default=field, **option_kwargs
                     )(command)
 
                 command = (optgroup.group(f"{backend_name} backend"))(command)
 
@@ -247,16 +273,18 @@
 def auth(username, password, scope, write):
     """Generate credentials for LRS HTTP basic authentification."""
     logger.info("Will generate credentials for user: %s", username)
 
     # Import required Pydantic models dynamically so that we don't create a
     # direct dependency between the CLI and the LRS
     # pylint: disable=invalid-name
-    ServerUsersCredentials = import_string("ralph.api.auth.ServerUsersCredentials")
-    UserCredentials = import_string("ralph.api.auth.UserCredentials")
+    ServerUsersCredentials = import_string(
+        "ralph.api.auth.basic.ServerUsersCredentials"
+    )
+    UserCredentials = import_string("ralph.api.auth.basic.UserCredentials")
 
     credentials = UserCredentials(
         username=username,
         hash=bcrypt.hashpw(
             bytes(password, encoding=settings.LOCALE_ENCODING), bcrypt.gensalt()
         ).decode("ascii"),
         scopes=scope,
@@ -423,30 +451,38 @@
     "-c",
     "--chunk-size",
     type=int,
     default=settings.DEFAULT_BACKEND_CHUNK_SIZE,
     help="Get events by chunks of size #",
 )
 @click.option(
+    "-t",
+    "--target",
+    type=str,
+    default=None,
+    help="Endpoint from which to fetch events (e.g. `/statements`)",
+)
+@click.option(
     "-q",
     "--query",
     type=JSONStringParamType(),
     default=None,
     help="Query object as a JSON string (database backends ONLY)",
 )
-def fetch(backend, archive, chunk_size, query, **options):
+def fetch(backend, archive, chunk_size, target, query, **options):
     """Fetch an archive or records from a configured backend."""
     logger.info(
         (
             "Fetching data from the configured %s backend "
-            "(archive: %s | chunk size: %s | query: %s)"
+            "(archive: %s | chunk size: %s | target: %s | query: %s)"
         ),
         backend,
         archive,
         chunk_size,
+        target,
         query,
     )
     logger.debug("Backend parameters: %s", options)
 
     backend_type = get_backend_type(settings.BACKENDS, backend)
     backend = get_backend_instance(backend_type, backend, options)
 
@@ -461,23 +497,37 @@
                 bytes(
                     json.dumps(document) if isinstance(document, dict) else document,
                     encoding="utf-8",
                 )
             )
     elif backend_type == settings.BACKENDS.STREAM:
         backend.stream(sys.stdout.buffer)
+    elif backend_type == settings.BACKENDS.HTTP:
+        for statement in backend.read(target=target, chunk_size=chunk_size):
+            click.echo(
+                bytes(
+                    json.dumps(statement) if isinstance(statement, dict) else statement,
+                    encoding="utf-8",
+                )
+            )
     elif backend_type is None:
         msg = "Cannot find an implemented backend type for backend %s"
         logger.error(msg, backend)
         raise UnsupportedBackendException(msg, backend)
 
 
-# pylint: disable=unnecessary-direct-lambda-call
+# pylint: disable=unnecessary-direct-lambda-call, too-many-arguments
 @click.argument("archive", required=False)
-@backends_options(backend_types=[settings.BACKENDS.DATABASE, settings.BACKENDS.STORAGE])
+@backends_options(
+    backend_types=[
+        settings.BACKENDS.DATABASE,
+        settings.BACKENDS.STORAGE,
+        settings.BACKENDS.HTTP,
+    ]
+)
 @click.option(
     "-c",
     "--chunk-size",
     type=int,
     default=settings.DEFAULT_BACKEND_CHUNK_SIZE,
     help="Get events by chunks of size #",
 )
@@ -491,26 +541,40 @@
 @click.option(
     "-I",
     "--ignore-errors",
     default=False,
     is_flag=True,
     help="Continue writing regardless of raised errors",
 )
-def push(backend, archive, chunk_size, force, ignore_errors, **options):
+@click.option(
+    "-t",
+    "--target",
+    type=str,
+    default=None,
+    help="Endpoint in which to push events (e.g. `statements`)",
+)
+def push(backend, archive, chunk_size, force, ignore_errors, target, **options):
     """Push an archive to a configured backend."""
     logger.info("Pushing archive %s to the configured %s backend", archive, backend)
     logger.debug("Backend parameters: %s", options)
 
     backend_type = get_backend_type(settings.BACKENDS, backend)
     backend = get_backend_instance(backend_type, backend, options)
 
     if backend_type == settings.BACKENDS.STORAGE:
         backend.write(sys.stdin.buffer, archive, overwrite=force)
     elif backend_type == settings.BACKENDS.DATABASE:
         backend.put(sys.stdin, chunk_size=chunk_size, ignore_errors=ignore_errors)
+    elif backend_type == settings.BACKENDS.HTTP:
+        backend.write(
+            target=target,
+            data=sys.stdin.buffer,
+            chunk_size=chunk_size,
+            ignore_errors=ignore_errors,
+        )
     elif backend_type is None:
         msg = "Cannot find an implemented backend type for backend %s"
         logger.error(msg, backend)
         raise UnsupportedBackendException(msg, backend)
 
 
 @backends_options(name="list", backend_types=[settings.BACKENDS.STORAGE])
```

### Comparing `ralph-malph-3.6.0/src/ralph/conf.py` & `ralph-malph-3.7.0/src/ralph/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Configurations for Ralph."""
 
 import io
+from enum import Enum
 from pathlib import Path
 from typing import List, Tuple, Union
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
@@ -14,15 +15,15 @@
 except ImportError:
     # If we use Ralph as a library and Click is not installed, we consider the
     # application directory to be the current directory. For non-CLI usage, it
     # has no consequences.
     from unittest.mock import Mock
 
     get_app_dir = Mock(return_value=".")
-from pydantic import AnyUrl, BaseModel, BaseSettings, Extra
+from pydantic import AnyHttpUrl, AnyUrl, BaseModel, BaseSettings, Extra, Field
 
 from .utils import import_string
 
 MODEL_PATH_SEPARATOR = "__"
 
 
 class BaseSettingsConfig:
@@ -76,42 +77,49 @@
         """Returns an instance of the settings item class using it's `_class_path`."""
         return import_string(self._class_path)(**init_parameters)
 
 
 # Active database backend Settings.
 
 
-class ClickhouseDatabaseBackendSettings(InstantiableSettingsItem):
-    """Pydantic model for ClickHouse database backend configuration settings."""
-
-    _class_path: str = "ralph.backends.database.clickhouse.ClickHouseDatabase"
-
-    HOST: str = "localhost"
-    PORT: int = 8123
-    DATABASE: str = "xapi"
-    EVENT_TABLE_NAME: str = "xapi_events_all"
-    USERNAME: str = None
-    PASSWORD: str = None
-    CLIENT_OPTIONS: dict = None
-
-
 class ClientOptions(BaseModel):
     """Pydantic model for additionnal client options."""
 
     class Config:  # pylint: disable=missing-class-docstring # noqa: D106
         extra = Extra.forbid
 
 
+class ClickhouseClientOptions(ClientOptions):
+    """Pydantic model for `clickhouse` client options."""
+
+    date_time_input_format: str = "best_effort"
+    allow_experimental_object_type: Literal[0, 1] = None
+
+
 class ESClientOptions(ClientOptions):
     """Pydantic model for Elasticsearch additionnal client options."""
 
     ca_certs: Path = None
     verify_certs: bool = None
 
 
+class ClickhouseDatabaseBackendSettings(InstantiableSettingsItem):
+    """Pydantic model for ClickHouse database backend configuration settings."""
+
+    _class_path: str = "ralph.backends.database.clickhouse.ClickHouseDatabase"
+
+    HOST: str = "localhost"
+    PORT: int = 8123
+    DATABASE: str = "xapi"
+    EVENT_TABLE_NAME: str = "xapi_events_all"
+    USERNAME: str = None
+    PASSWORD: str = None
+    CLIENT_OPTIONS: ClickhouseClientOptions = None
+
+
 class MongoClientOptions(ClientOptions):
     """Pydantic model for MongoDB additionnal client options."""
 
     document_class: str = None
     tz_aware: bool = None
 
 
@@ -141,14 +149,50 @@
     """Pydantic model for database backend configuration settings."""
 
     ES: ESDatabaseBackendSettings = ESDatabaseBackendSettings()
     MONGO: MongoDatabaseBackendSettings = MongoDatabaseBackendSettings()
     CLICKHOUSE: ClickhouseDatabaseBackendSettings = ClickhouseDatabaseBackendSettings()
 
 
+# Active HTTP backend Settings.
+
+
+class HeadersParameters(BaseModel):
+    """Pydantic model for headers parameters."""
+
+    class Config:  # pylint: disable=missing-class-docstring # noqa: D106
+        extra = Extra.allow
+
+
+class LRSHeaders(HeadersParameters):
+    """Pydantic model for LRS headers."""
+
+    X_EXPERIENCE_API_VERSION: str = "1.0.3"
+    CONTENT_TYPE: str = "application/json"
+
+
+class LRSHTTPBackendSettings(InstantiableSettingsItem):
+    """Pydantic model for LRS HTTP backend configuration settings."""
+
+    _class_path: str = "ralph.backends.http.lrs.LRSHTTP"
+
+    BASE_URL: AnyHttpUrl = Field("http://0.0.0.0:8100")
+    USERNAME: str = "ralph"
+    PASSWORD: str = "secret"
+    HEADERS: LRSHeaders = LRSHeaders()
+    STATUS_ENDPOINT: str = "/__heartbeat__"
+    STATEMENTS_ENDPOINT: str = "/xAPI/statements"
+
+
+class HTTPBackendSettings(BaseModel):
+    """Pydantic model for HTTP backend configuration settings."""
+
+    LRS: LRSHTTPBackendSettings = LRSHTTPBackendSettings()
+
+
 # Active storage backend Settings.
 
 
 class FSStorageBackendSettings(InstantiableSettingsItem):
     """Pydantic model for FileSystem storage backend configuration settings."""
 
     _class_path: str = "ralph.backends.storage.fs.FSStorage"
@@ -192,14 +236,15 @@
     _class_path: str = "ralph.backends.storage.s3.S3Storage"
 
     ACCESS_KEY_ID: str = None
     SECRET_ACCESS_KEY: str = None
     SESSION_TOKEN: str = None
     DEFAULT_REGION: str = None
     BUCKET_NAME: str = None
+    ENDPOINT_URL: str = None
 
 
 class StorageBackendSettings(BaseModel):
     """Pydantic model for storage backend configuration settings."""
 
     LDP: LDPStorageBackendSettings = LDPStorageBackendSettings()
     FS: FSStorageBackendSettings = FSStorageBackendSettings()
@@ -227,14 +272,15 @@
 # Active backend Settings.
 
 
 class BackendSettings(BaseModel):
     """Pydantic model for backends configuration settings."""
 
     DATABASE: DatabaseBackendSettings = DatabaseBackendSettings()
+    HTTP: HTTPBackendSettings = HTTPBackendSettings()
     STORAGE: StorageBackendSettings = StorageBackendSettings()
     STREAM: StreamBackendSettings = StreamBackendSettings()
 
 
 # Active parser Settings.
 
 
@@ -276,16 +322,24 @@
 
     class Config(BaseSettingsConfig):
         """Pydantic Configuration."""
 
         env_file = ".env"
         env_file_encoding = core_settings.LOCALE_ENCODING
 
+    class AuthBackends(Enum):
+        """Enum of the authentication backends."""
+
+        BASIC = "basic"
+        OIDC = "oidc"
+
     _CORE: CoreSettings = core_settings
     AUTH_FILE: Path = _CORE.APP_DIR / "auth.json"
+    AUTH_CACHE_MAX_SIZE = 100
+    AUTH_CACHE_TTL = 3600
     BACKENDS: BackendSettings = BackendSettings()
     CONVERTER_EDX_XAPI_UUID_NAMESPACE: str = None
     DEFAULT_BACKEND_CHUNK_SIZE: int = 500
     EXECUTION_ENVIRONMENT: str = "development"
     HISTORY_FILE: Path = _CORE.APP_DIR / "history.json"
     LOGGING: dict = {
         "version": 1,
@@ -315,14 +369,17 @@
             "uvicorn": {
                 "handlers": ["console"],
                 "level": "INFO",
             },
         },
     }
     PARSERS: ParserSettings = ParserSettings()
+    RUNSERVER_AUTH_BACKEND: AuthBackends = AuthBackends.BASIC
+    RUNSERVER_AUTH_OIDC_AUDIENCE: str = None
+    RUNSERVER_AUTH_OIDC_ISSUER_URI: AnyHttpUrl = None
     RUNSERVER_BACKEND: Literal["clickhouse", "es", "mongo"] = "es"
     RUNSERVER_HOST: str = "0.0.0.0"  # nosec
     RUNSERVER_MAX_SEARCH_HITS_COUNT: int = 100
     RUNSERVER_POINT_IN_TIME_KEEP_ALIVE: str = "1m"
     RUNSERVER_PORT: int = 8100
     SENTRY_CLI_TRACES_SAMPLE_RATE: float = 1.0
     SENTRY_DSN: str = None
```

### Comparing `ralph-malph-3.6.0/src/ralph/exceptions.py` & `ralph-malph-3.7.0/src/ralph/exceptions.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/filters.py` & `ralph-malph-3.7.0/src/ralph/filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/converter.py` & `ralph-malph-3.7.0/src/ralph/models/converter.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/__init__.py` & `ralph-malph-3.7.0/src/ralph/models/edx/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/base.py` & `ralph-malph-3.7.0/src/ralph/models/edx/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/browser.py` & `ralph-malph-3.7.0/src/ralph/models/edx/browser.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/base.py` & `ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Base xAPI Converter."""
 
 import re
 from uuid import UUID, uuid5
 
 from ralph.exceptions import ConfigurationException
 from ralph.models.converter import BaseConversionSet, ConversionItem
-from ralph.models.xapi.constants import (
-    EXTENSION_COURSE_ID,
-    EXTENSION_MODULE_ID,
-    EXTENSION_SCHOOL_ID,
+from ralph.models.xapi.concepts.constants.acrossx_profile import (
+    CONTEXT_EXTENSION_SCHOOL_ID,
+)
+from ralph.models.xapi.concepts.constants.scorm_profile import (
+    CONTEXT_EXTENSION_COURSE_ID,
+    CONTEXT_EXTENSION_MODULE_ID,
 )
 
 
 class BaseXapiConverter(BaseConversionSet):
     """Base xAPI Converter.
 
     WARNING: The converter may not include the following edX fields:
@@ -47,24 +49,24 @@
             ),
             ConversionItem(
                 "actor__account__name",
                 "context__user_id",
                 lambda user_id: str(user_id) if user_id else "anonymous",
             ),
             ConversionItem(
-                "object__definition__extensions__" + EXTENSION_SCHOOL_ID,
+                "object__definition__extensions__" + CONTEXT_EXTENSION_SCHOOL_ID,
                 "context__org_id",
             ),
             ConversionItem(
-                "object__definition__extensions__" + EXTENSION_COURSE_ID,
+                "object__definition__extensions__" + CONTEXT_EXTENSION_COURSE_ID,
                 "context__course_id",
                 (self.parse_course_id, lambda x: x["course"]),
             ),
             ConversionItem(
-                "object__definition__extensions__" + EXTENSION_MODULE_ID,
+                "object__definition__extensions__" + CONTEXT_EXTENSION_MODULE_ID,
                 "context__course_id",
                 (self.parse_course_id, lambda x: x["module"]),
             ),
             ConversionItem("timestamp", "time"),
         }
 
     @staticmethod
```

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/navigational.py` & `ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/navigational.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/server.py` & `ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/video.py` & `ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/video.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from ralph.models.edx.video.statements import (
     UILoadVideo,
     UIPauseVideo,
     UIPlayVideo,
     UISeekVideo,
     UIStopVideo,
 )
-from ralph.models.xapi.constants import LANG_EN_US_DISPLAY
-from ralph.models.xapi.video.constants import (
-    VIDEO_EXTENSION_LENGTH,
-    VIDEO_EXTENSION_PROGRESS,
-    VIDEO_EXTENSION_SESSION_ID,
-    VIDEO_EXTENSION_TIME,
-    VIDEO_EXTENSION_TIME_FROM,
-    VIDEO_EXTENSION_TIME_TO,
-    VIDEO_EXTENSION_USER_AGENT,
+from ralph.models.xapi.concepts.constants.video import (
+    CONTEXT_EXTENSION_LENGTH,
+    CONTEXT_EXTENSION_SESSION_ID,
+    CONTEXT_EXTENSION_USER_AGENT,
+    RESULT_EXTENSION_PROGRESS,
+    RESULT_EXTENSION_TIME,
+    RESULT_EXTENSION_TIME_FROM,
+    RESULT_EXTENSION_TIME_TO,
 )
+from ralph.models.xapi.constants import LANG_EN_US_DISPLAY
 from ralph.models.xapi.video.statements import (
     VideoInitialized,
     VideoPaused,
     VideoPlayed,
     VideoSeeked,
     VideoTerminated,
 )
@@ -36,27 +36,27 @@
         """Returns a set of ConversionItems used for conversion."""
         conversion_items = super()._get_conversion_items()
         return conversion_items.union(
             {
                 ConversionItem(
                     "object__definition__name",
                     "event__id",
-                    lambda id: {LANG_EN_US_DISPLAY.__args__[0]: id},
+                    lambda id: {LANG_EN_US_DISPLAY: id},
                 ),
                 ConversionItem(
                     "object__id",
                     None,
                     lambda event: self.platform_url
                     + "/xblock/block-v1:"
                     + event["context"]["course_id"]
                     + "-course-v1:+type@video+block@"
                     + event["event"]["id"],
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_SESSION_ID,
+                    "context__extensions__" + CONTEXT_EXTENSION_SESSION_ID,
                     "session",
                 ),
             },
         )
 
 
 class UILoadVideoToVideoInitialized(VideoBaseXapiConverter):
@@ -67,27 +67,27 @@
 
     def _get_conversion_items(self):
         """Returns a set of ConversionItems used for conversion."""
         conversion_items = super()._get_conversion_items()
         return conversion_items.union(
             {
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_LENGTH,
+                    "context__extensions__" + CONTEXT_EXTENSION_LENGTH,
                     None,
                     # Set the video length to null by default.
                     # This information is mandatory in the xAPI template
                     # and does not exist in the edX `load_video` event model.
                     lambda _: 0.0,
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_SESSION_ID,
+                    "context__extensions__" + CONTEXT_EXTENSION_SESSION_ID,
                     "session",
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_USER_AGENT, "agent"
+                    "context__extensions__" + CONTEXT_EXTENSION_USER_AGENT, "agent"
                 ),
             },
         )
 
 
 class UIPlayVideoToVideoPlayed(VideoBaseXapiConverter):
     """Converts a common edX `play_video` event to xAPI."""
@@ -97,19 +97,19 @@
 
     def _get_conversion_items(self):
         """Returns a set of ConversionItems used for conversion."""
         conversion_items = super()._get_conversion_items()
         return conversion_items.union(
             {
                 ConversionItem(
-                    "result__extensions__" + VIDEO_EXTENSION_TIME,
+                    "result__extensions__" + RESULT_EXTENSION_TIME,
                     "event__currentTime",
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_SESSION_ID,
+                    "context__extensions__" + CONTEXT_EXTENSION_SESSION_ID,
                     "session",
                 ),
             },
         )
 
 
 class UIPauseVideoToVideoPaused(VideoBaseXapiConverter):
@@ -120,27 +120,27 @@
 
     def _get_conversion_items(self):
         """Returns a set of ConversionItems used for conversion."""
         conversion_items = super()._get_conversion_items()
         return conversion_items.union(
             {
                 ConversionItem(
-                    "result__extensions__" + VIDEO_EXTENSION_TIME,
+                    "result__extensions__" + RESULT_EXTENSION_TIME,
                     "event__currentTime",
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_LENGTH,
+                    "context__extensions__" + CONTEXT_EXTENSION_LENGTH,
                     None,
                     # Set the video length to null by default.
                     # This information is mandatory in the xAPI template
                     # and does not exist in the edX `pause_video` event model.
                     lambda _: 0.0,
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_SESSION_ID,
+                    "context__extensions__" + CONTEXT_EXTENSION_SESSION_ID,
                     "session",
                 ),
             },
         )
 
 
 class UIStopVideoToVideoTerminated(VideoBaseXapiConverter):
@@ -151,35 +151,35 @@
 
     def _get_conversion_items(self):
         """Returns a set of ConversionItems used for conversion."""
         conversion_items = super()._get_conversion_items()
         return conversion_items.union(
             {
                 ConversionItem(
-                    "result__extensions__" + VIDEO_EXTENSION_TIME,
+                    "result__extensions__" + RESULT_EXTENSION_TIME,
                     "event__currentTime",
                 ),
                 ConversionItem(
-                    "result__extensions__" + VIDEO_EXTENSION_PROGRESS,
+                    "result__extensions__" + RESULT_EXTENSION_PROGRESS,
                     None,
                     # Set the video progress to null by default.
                     # This information is mandatory in the xAPI template
                     # and does not exist in the edX `stop_video` event model.
                     lambda _: 0.0,
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_LENGTH,
+                    "context__extensions__" + CONTEXT_EXTENSION_LENGTH,
                     None,
                     # Set the video length to null by default.
                     # This information is mandatory in the xAPI template
                     # and does not exist in the edX `stop_video` event model.
                     lambda _: 0.0,
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_SESSION_ID,
+                    "context__extensions__" + CONTEXT_EXTENSION_SESSION_ID,
                     "session",
                 ),
             },
         )
 
 
 class UISeekVideoToVideoSeeked(VideoBaseXapiConverter):
@@ -190,20 +190,20 @@
 
     def _get_conversion_items(self):
         """Returns a set of ConversionItems used for conversion."""
         conversion_items = super()._get_conversion_items()
         return conversion_items.union(
             {
                 ConversionItem(
-                    "result__extensions__" + VIDEO_EXTENSION_TIME_FROM,
+                    "result__extensions__" + RESULT_EXTENSION_TIME_FROM,
                     "event__old_time",
                 ),
                 ConversionItem(
-                    "result__extensions__" + VIDEO_EXTENSION_TIME_TO,
+                    "result__extensions__" + RESULT_EXTENSION_TIME_TO,
                     "event__new_time",
                 ),
                 ConversionItem(
-                    "context__extensions__" + VIDEO_EXTENSION_SESSION_ID,
+                    "context__extensions__" + CONTEXT_EXTENSION_SESSION_ID,
                     "session",
                 ),
             },
         )
```

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/contexts.py` & `ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/events.py` & `ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/enrollment/statements.py` & `ralph-malph-3.7.0/src/ralph/models/edx/enrollment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/navigational/fields/events.py` & `ralph-malph-3.7.0/src/ralph/models/edx/navigational/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/navigational/statements.py` & `ralph-malph-3.7.0/src/ralph/models/edx/navigational/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/fields/events.py` & `ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/statements.py` & `ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/server.py` & `ralph-malph-3.7.0/src/ralph/models/edx/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/fields/events.py` & `ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/statements.py` & `ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/video/fields/events.py` & `ralph-malph-3.7.0/src/ralph/models/edx/video/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/edx/video/statements.py` & `ralph-malph-3.7.0/src/ralph/models/edx/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/selector.py` & `ralph-malph-3.7.0/src/ralph/models/selector.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/validator.py` & `ralph-malph-3.7.0/src/ralph/models/validator.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/xapi/config.py` & `ralph-malph-3.7.0/src/ralph/models/xapi/config.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/models/xapi/fields/attachments.py` & `ralph-malph-3.7.0/src/ralph/models/xapi/base/attachments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Common xAPI attachments field definitions."""
+"""Base xAPI `Attachments` definitions."""
 
 from typing import Optional
 
 from pydantic import AnyUrl
 
 from ..config import BaseModelWithConfig
 from .common import IRI, LanguageMap
 
 
-class AttachmentField(BaseModelWithConfig):
-    """Pydantic model for `attachment` field.
+class BaseXapiAttachment(BaseModelWithConfig):
+    """Pydantic model for `attachment` property.
 
     Attributes:
         usageType (IRI): Identifies the usage of this Attachment.
         display (LanguageMap): Consists of the Attachment's title.
         description (LanguageMap): Consists of the Attachment's description.
         contentType (str): Consists of the Attachment's content type.
         length (int): Consists of the length of the Attachment's data in octets.
```

### Comparing `ralph-malph-3.6.0/src/ralph/models/xapi/fields/common.py` & `ralph-malph-3.7.0/src/ralph/models/xapi/base/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Common xAPI field definitions."""
+"""Common for xAPI base definitions."""
 
 from typing import Dict
 
 from langcodes import tag_is_valid
 from pydantic import StrictStr, validate_email
 from rfc3987 import parse
```

### Comparing `ralph-malph-3.6.0/src/ralph/models/xapi/fields/results.py` & `ralph-malph-3.7.0/src/ralph/models/xapi/base/results.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Common xAPI result field definitions."""
+"""Base xAPI `Result` definitions."""
 
 from datetime import timedelta
 from decimal import Decimal
 from typing import Dict, Optional, Union
 
 from pydantic import StrictBool, StrictStr, conint, root_validator
 
 from ..config import BaseModelWithConfig
 from .common import IRI
 
 
-class ScoreResultField(BaseModelWithConfig):
-    """Pydantic model for `results.score` field.
+class BaseXapiResultScore(BaseModelWithConfig):
+    """Pydantic model for result `score` property.
 
     Attributes:
         scaled (int): Consists of the normalized score related to the experience.
         raw (Decimal): Consists of the non-normalized score achieved by the Actor.
         min (Decimal): Consists of lowest possible score.
         max (Decimal): Consists of highest possible score.
     """
@@ -41,25 +41,26 @@
         if max_value:
             if raw_value and raw_value > max_value:
                 raise ValueError("raw cannot be greater than max")
 
         return values
 
 
-class ResultField(BaseModelWithConfig):
-    """Pydantic model for `result` field.
+class BaseXapiResult(BaseModelWithConfig):
+    """Pydantic model for `result` property.
 
     Attributes:
-        score (ScoreResultField): See ScoreResultField.
+        score (dict): See BaseXapiResultScore.
         success (bool): Indicates whether the attempt on the Activity was successful.
         completion (bool): Indicates whether the Activity was completed.
         response (str): Consists of the response for the given Activity.
-        duration (str): Consists of the duration over which the Statement occurred.
+        duration (timedelta): Consists of the duration over which the Statement
+            occurred.
         extensions (dict): Consists of a dictionary of other properties as needed.
     """
 
-    score: Optional[ScoreResultField]
+    score: Optional[BaseXapiResultScore]
     success: Optional[StrictBool]
     completion: Optional[StrictBool]
     response: Optional[StrictStr]
     duration: Optional[timedelta]
     extensions: Optional[Dict[IRI, Union[str, int, bool, list, dict, None]]]
```

### Comparing `ralph-malph-3.6.0/src/ralph/models/xapi/fields/unnested_objects.py` & `ralph-malph-3.7.0/src/ralph/models/xapi/base/unnested_objects.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Common xAPI object field definitions."""
+"""Base xAPI `Object` definitions (1)."""
 
 from typing import Dict, List, Optional, Union
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
@@ -11,46 +11,46 @@
 
 from pydantic import AnyUrl, StrictStr, constr, validator
 
 from ..config import BaseModelWithConfig
 from .common import IRI, LanguageMap
 
 
-class ObjectDefinitionField(BaseModelWithConfig):
-    """Pydantic model for `object.definition` field.
+class BaseXapiActivityDefinition(BaseModelWithConfig):
+    """Pydantic model for `Activity` type `definition` property.
 
     Attributes:
         name (LanguageMap): Consists of the human readable/visual name of the Activity.
         description (LanguageMap): Consists of a description of the Activity.
         type (IRI): Consists of the type of the Activity.
         moreInfo (URL): Consists of an URL to a document about the Activity.
-        extensions (Dict): Consists of a dictionary of other properties as needed.
+        extensions (dict): Consists of a dictionary of other properties as needed.
     """
 
     name: Optional[LanguageMap]
     description: Optional[LanguageMap]
     type: Optional[IRI]
     moreInfo: Optional[AnyUrl]
     extensions: Optional[Dict[IRI, Union[str, int, bool, list, dict, None]]]
 
 
-class InteractionComponent(BaseModelWithConfig):
+class BaseXapiInteractionComponent(BaseModelWithConfig):
     """Pydantic model for an interaction component.
 
     Attributes:
         id (str): Consists of an identifier of the interaction component.
         description (LanguageMap): Consists of the description of the interaction.
     """
 
     id: constr(regex=r"^[^\s]+$")  # noqa:F722
     description: Optional[LanguageMap]
 
 
-class InteractionObjectDefinitionField(ObjectDefinitionField):
-    """Pydantic model for `object.definition` field.
+class BaseXapiActivityInteractionDefinition(BaseXapiActivityDefinition):
+    """Pydantic model for `Activity` type `definition` property.
 
     It is defined for field with interaction properties.
 
     Attributes:
         interactionType (str): Consists of the type of the interaction.
         correctResponsesPattern (list): Consists of a pattern for the correct response.
         choices (list): Consists of a list of selectable choices.
@@ -69,52 +69,54 @@
         "performance",
         "sequencing",
         "likert",
         "numeric",
         "other",
     ]
     correctResponsesPattern: Optional[List[StrictStr]]
-    choices: Optional[List[InteractionComponent]]
-    scale: Optional[List[InteractionComponent]]
-    source: Optional[List[InteractionComponent]]
-    target: Optional[List[InteractionComponent]]
-    steps: Optional[List[InteractionComponent]]
+    choices: Optional[List[BaseXapiInteractionComponent]]
+    scale: Optional[List[BaseXapiInteractionComponent]]
+    source: Optional[List[BaseXapiInteractionComponent]]
+    target: Optional[List[BaseXapiInteractionComponent]]
+    steps: Optional[List[BaseXapiInteractionComponent]]
 
     @validator("choices", "scale", "source", "target", "steps")
     @classmethod
     def check_unique_ids(cls, value):
         """Checks the uniqueness of interaction components IDs."""
         if len(value) != len({x.id for x in value}):
             raise ValueError("Duplicate InteractionComponents are not valid")
 
 
-class ActivityObjectField(BaseModelWithConfig):
-    """Pydantic model for `object` field.
-
-    It is defined for Activity type.
+class BaseXapiActivity(BaseModelWithConfig):
+    """Pydantic model for `Activity` type property.
 
     Attributes:
-        objectType (str): Consists of the value `Activity`.
         id (IRI): Consists of an identifier for a single unique Activity.
-        definition (dict): See ObjectDefinitionField.
+        objectType (str): Consists of the value `Activity`.
+        definition (dict): See BaseXapiActivityDefinition and
+            BaseXapiActivityInteractionDefinition.
     """
 
     id: IRI
     objectType: Optional[Literal["Activity"]]
-    definition: Optional[Union[ObjectDefinitionField, InteractionObjectDefinitionField]]
-
+    definition: Optional[
+        Union[
+            BaseXapiActivityDefinition,
+            BaseXapiActivityInteractionDefinition,
+        ]
+    ]
 
-class StatementRefObjectField(BaseModelWithConfig):
-    """Pydantic model for `object` field.
 
-    It is defined for StatementRef type.
+class BaseXapiStatementRef(BaseModelWithConfig):
+    """Pydantic model for `StatementRef` type property.
 
     Attributes:
         objectType (str): Consists of the value `StatementRef`.
         id (UUID): Consists of the UUID of the referenced statement.
     """
 
     id: UUID
     objectType: Literal["StatementRef"]
 
 
-UnnestedObjectField = Union[ActivityObjectField, StatementRefObjectField]
+BaseXapiUnnestedObject = Union[BaseXapiActivity, BaseXapiStatementRef]
```

### Comparing `ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/contexts.py` & `ralph-malph-3.7.0/src/ralph/models/xapi/video/contexts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,88 @@
 """Video xAPI events context fields definitions."""
 
-from typing import Dict, List, Optional
+from typing import List, Optional, Union
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from uuid import UUID
 
 from pydantic import Field, NonNegativeFloat
 
-from ...config import BaseExtensionModelWithConfig
-from ...fields.contexts import ContextActivitiesContextField, ContextField
-from ..constants import (
-    VIDEO_CONTEXT_CATEGORY,
-    VIDEO_EXTENSION_CC_ENABLED,
-    VIDEO_EXTENSION_CC_SUBTITLE_LANG,
-    VIDEO_EXTENSION_COMPLETION_THRESHOLD,
-    VIDEO_EXTENSION_FULL_SCREEN,
-    VIDEO_EXTENSION_LENGTH,
-    VIDEO_EXTENSION_SCREEN_SIZE,
-    VIDEO_EXTENSION_SESSION_ID,
-    VIDEO_EXTENSION_SPEED,
-    VIDEO_EXTENSION_USER_AGENT,
-    VIDEO_EXTENSION_VIDEO_PLAYBACK_SIZE,
-    VIDEO_EXTENSION_VOLUME,
+from ..base.contexts import BaseXapiContext, BaseXapiContextContextActivities
+from ..base.unnested_objects import BaseXapiActivity
+from ..concepts.activity_types.scorm_profile import ProfileActivity
+from ..concepts.constants.video import (
+    CONTEXT_EXTENSION_CC_ENABLED,
+    CONTEXT_EXTENSION_CC_SUBTITLE_LANG,
+    CONTEXT_EXTENSION_COMPLETION_THRESHOLD,
+    CONTEXT_EXTENSION_FULL_SCREEN,
+    CONTEXT_EXTENSION_LENGTH,
+    CONTEXT_EXTENSION_SCREEN_SIZE,
+    CONTEXT_EXTENSION_SESSION_ID,
+    CONTEXT_EXTENSION_SPEED,
+    CONTEXT_EXTENSION_USER_AGENT,
+    CONTEXT_EXTENSION_VIDEO_PLAYBACK_SIZE,
+    CONTEXT_EXTENSION_VOLUME,
 )
+from ..config import BaseExtensionModelWithConfig
 
 
-class VideoContextActivitiesField(ContextActivitiesContextField):
-    """Pydantic model for video `contextActivities` field.
+class VideoContextContextActivitiesCategory(BaseXapiActivity):
+    # noqa: D205, D415
+    """Pydantic model for video `context`.`contextActivities`.`category`
+    property.
 
     Attributes:
-        category (List): Consists of a list containing the dictionary
-            {"id": "https://w3id.org/xapi/video"}.
+        id (str): Consists of the value `https://w3id.org/xapi/video`.
+        definition (dict): see ProfileActivity.
     """
 
-    category: List[Dict[Literal["id"], VIDEO_CONTEXT_CATEGORY]] = [
-        {"id": VIDEO_CONTEXT_CATEGORY.__args__[0]}
+    id: Literal["https://w3id.org/xapi/video"] = "https://w3id.org/xapi/video"
+    definition: ProfileActivity
+
+
+class VideoContextContextActivities(BaseXapiContextContextActivities):
+    """Pydantic model for video `context`.`contextActivities` property.
+
+    Attributes:
+        category (list): see VideoContextContextActivitiesCategory.
+    """
+
+    category: Union[
+        VideoContextContextActivitiesCategory,
+        List[VideoContextContextActivitiesCategory],
     ]
 
 
-class BaseVideoContextField(ContextField):
-    """Pydantic model for video core `context` field.
+class BaseVideoContext(BaseXapiContext):
+    """Pydantic model for video core `context` property.
 
     Attributes:
-        contextActivities (dict): see VideoContextActivitiesField.
+        contextActivities (dict): see VideoContextContextActivities.
     """
 
-    contextActivities: Optional[VideoContextActivitiesField]
+    contextActivities: Optional[VideoContextContextActivities]
 
 
-class VideoContextExtensionsField(BaseExtensionModelWithConfig):
-    """Pydantic model for video core `context`.`extensions` field.
+class VideoContextExtensions(BaseExtensionModelWithConfig):
+    """Pydantic model for video core context `extensions` property.
 
     Attributes:
         session (uuid): Consists of the ID of the active session.
     """
 
-    session_id: Optional[UUID] = Field(alias=VIDEO_EXTENSION_SESSION_ID)
+    session_id: Optional[UUID] = Field(alias=CONTEXT_EXTENSION_SESSION_ID)
 
 
-class VideoInitializedContextExtensionsField(VideoContextExtensionsField):
-    """Pydantic model for video initialized `context`.`extensions` field.
+class VideoInitializedContextExtensions(VideoContextExtensions):
+    """Pydantic model for video initialized `context` `extensions` property.
 
     Attributes:
         length (float): Consists of the length of the video.
         ccSubtitleEnabled (bool): Indicates whether subtitle or closed captioning is
             enabled.
         ccSubtitleLanguage (str): Consists of the language of subtitle or closed
             captioning.
@@ -80,162 +95,168 @@
         userAgent (str): Consists of the User Agent string of the browser,
             if the video is launched in browser.
         volume (int): Consists of the volume of the video.
         completionThreshold (float): Consists of the percentage of media that should be
             consumed to trigger a completion.
     """
 
-    length: NonNegativeFloat = Field(alias=VIDEO_EXTENSION_LENGTH)
-    ccSubtitleEnabled: Optional[bool] = Field(alias=VIDEO_EXTENSION_CC_ENABLED)
-    ccSubtitleLang: Optional[str] = Field(alias=VIDEO_EXTENSION_CC_SUBTITLE_LANG)
-    fullScreen: Optional[bool] = Field(alias=VIDEO_EXTENSION_FULL_SCREEN)
-    screenSize: Optional[str] = Field(alias=VIDEO_EXTENSION_SCREEN_SIZE)
-    videoPlaybackSize: Optional[str] = Field(alias=VIDEO_EXTENSION_VIDEO_PLAYBACK_SIZE)
-    speed: Optional[str] = Field(alias=VIDEO_EXTENSION_SPEED)
-    userAgent: Optional[str] = Field(alias=VIDEO_EXTENSION_USER_AGENT)
-    volume: Optional[int] = Field(alias=VIDEO_EXTENSION_VOLUME)
+    length: NonNegativeFloat = Field(alias=CONTEXT_EXTENSION_LENGTH)
+    ccSubtitleEnabled: Optional[bool] = Field(alias=CONTEXT_EXTENSION_CC_ENABLED)
+    ccSubtitleLang: Optional[str] = Field(alias=CONTEXT_EXTENSION_CC_SUBTITLE_LANG)
+    fullScreen: Optional[bool] = Field(alias=CONTEXT_EXTENSION_FULL_SCREEN)
+    screenSize: Optional[str] = Field(alias=CONTEXT_EXTENSION_SCREEN_SIZE)
+    videoPlaybackSize: Optional[str] = Field(
+        alias=CONTEXT_EXTENSION_VIDEO_PLAYBACK_SIZE
+    )
+    speed: Optional[str] = Field(alias=CONTEXT_EXTENSION_SPEED)
+    userAgent: Optional[str] = Field(alias=CONTEXT_EXTENSION_USER_AGENT)
+    volume: Optional[int] = Field(alias=CONTEXT_EXTENSION_VOLUME)
     completionThreshold: Optional[float] = Field(
-        alias=VIDEO_EXTENSION_COMPLETION_THRESHOLD
+        alias=CONTEXT_EXTENSION_COMPLETION_THRESHOLD
     )
 
 
-class VideoBrowsingContextExtensionsField(VideoContextExtensionsField):
-    """Pydantic model for video browsing `context`.`extensions` field.
+class VideoBrowsingContextExtensions(VideoContextExtensions):
+    """Pydantic model for video browsing `context`.`extensions` property.
 
     Such field is used in `paused`, `completed` and `terminated` events.
 
     Attributes:
         completionThreshold (float): Consists of the percentage of media that should
             be consumed to trigger a completion.
         length (float): Consists of the length of the video.
     """
 
-    length: NonNegativeFloat = Field(alias=VIDEO_EXTENSION_LENGTH)
+    length: NonNegativeFloat = Field(alias=CONTEXT_EXTENSION_LENGTH)
     completionThreshold: Optional[float] = Field(
-        alias=VIDEO_EXTENSION_COMPLETION_THRESHOLD
+        alias=CONTEXT_EXTENSION_COMPLETION_THRESHOLD
     )
 
 
-class VideoEnableClosedCaptioningContextExtensionsField(VideoContextExtensionsField):
+class VideoEnableClosedCaptioningContextExtensions(VideoContextExtensions):
     """Represents the context.extensions field for video `interacted` xAPI statement.
 
     Attributes:
         ccSubtitleLanguage (str): Consists of the language of subtitle or closed
             captioning.
     """
 
-    ccSubtitleLanguage: str = Field(alias=VIDEO_EXTENSION_CC_SUBTITLE_LANG)
+    ccSubtitleLanguage: str = Field(alias=CONTEXT_EXTENSION_CC_SUBTITLE_LANG)
 
 
-class VideoVolumeChangeInteractionContextExtensionsField(VideoContextExtensionsField):
-    """Pydantic model for video volume change interaction `context`.`extensions` field.
+class VideoVolumeChangeInteractionContextExtensions(VideoContextExtensions):
+    # noqa: D205, D415
+    """Pydantic model for video volume change interaction `context`.`extensions`
+    property.
 
     Attributes:
         volume (int): Consists of the volume of the video.
     """
 
-    volume: int = Field(alias=VIDEO_EXTENSION_VOLUME)
+    volume: int = Field(alias=CONTEXT_EXTENSION_VOLUME)
 
 
-class VideoScreenChangeInteractionContextExtensionsField(VideoContextExtensionsField):
-    """Pydantic model for video screen change interaction `context`.`extensions` field.
+class VideoScreenChangeInteractionContextExtensions(VideoContextExtensions):
+    # noqa: D205, D415
+    """Pydantic model for video screen change interaction `context`.`extensions`
+    property.
 
     Attributes:
         fullScreen (bool): Indicates whether the video is played in full screen mode.
         screenSize (str): Expresses the total available screen size for Video playback.
         videoPlaybackSize (str): Consists of the size in Width x Height of the video as
             viewed by the user.
     """
 
-    fullScreen: bool = Field(alias=VIDEO_EXTENSION_FULL_SCREEN)
-    screenSize: str = Field(alias=VIDEO_EXTENSION_SCREEN_SIZE)
-    videoPlaybackSize: str = Field(alias=VIDEO_EXTENSION_VIDEO_PLAYBACK_SIZE)
+    fullScreen: bool = Field(alias=CONTEXT_EXTENSION_FULL_SCREEN)
+    screenSize: str = Field(alias=CONTEXT_EXTENSION_SCREEN_SIZE)
+    videoPlaybackSize: str = Field(alias=CONTEXT_EXTENSION_VIDEO_PLAYBACK_SIZE)
 
 
-class VideoInitializedContextField(BaseVideoContextField):
-    """Pydantic model for video initialized `context` field.
+class VideoInitializedContext(BaseVideoContext):
+    """Pydantic model for video initialized `context` property.
 
     Attributes:
-        extensions (dict): See VideoInitializedContextExtensionsField.
+        extensions (dict): See VideoInitializedContextExtensions.
     """
 
-    extensions: VideoInitializedContextExtensionsField
+    extensions: VideoInitializedContextExtensions
 
 
-class VideoPlayedContextField(BaseVideoContextField):
-    """Pydantic model for video played `context` field.
+class VideoPlayedContext(BaseVideoContext):
+    """Pydantic model for video played `context` property.
 
     Attributes:
-        extensions (dict): See VideoContextExtensionsField.
+        extensions (dict): See VideoContextExtensions.
     """
 
-    extensions: Optional[VideoContextExtensionsField]
+    extensions: Optional[VideoContextExtensions]
 
 
-class VideoPausedContextField(BaseVideoContextField):
-    """Pydantic model for video paused `context` field.
+class VideoPausedContext(BaseVideoContext):
+    """Pydantic model for video paused `context` property.
 
     Attributes:
-        extensions (dict): See VideoBrowsingContextExtensionsField.
+        extensions (dict): See VideoBrowsingContextExtensions.
     """
 
-    extensions: VideoBrowsingContextExtensionsField
+    extensions: VideoBrowsingContextExtensions
 
 
-class VideoSeekedContextField(BaseVideoContextField):
-    """Pydantic model for video seeked `context` field.
+class VideoSeekedContext(BaseVideoContext):
+    """Pydantic model for video seeked `context` property.
 
     Attributes:
-        extensions (dict): See VideoContextExtensionsField.
+        extensions (dict): See VideoContextExtensions.
     """
 
-    extensions: Optional[VideoContextExtensionsField]
+    extensions: Optional[VideoContextExtensions]
 
 
-class VideoCompletedContextField(BaseVideoContextField):
-    """Pydantic model for video completed `context` field.
+class VideoCompletedContext(BaseVideoContext):
+    """Pydantic model for video completed `context` property.
 
     Attributes:
-        extensions (dict): See VideoBrowsingContextExtensionsField.
+        extensions (dict): See VideoBrowsingContextExtensions.
     """
 
-    extensions: VideoBrowsingContextExtensionsField
+    extensions: VideoBrowsingContextExtensions
 
 
-class VideoTerminatedContextField(BaseVideoContextField):
-    """Pydantic model for video terminated `context` field.
+class VideoTerminatedContext(BaseVideoContext):
+    """Pydantic model for video terminated `context` property.
 
     Attributes:
-        extensions (dict): See VideoBrowsingContextExtensionsField.
+        extensions (dict): See VideoBrowsingContextExtensions.
     """
 
-    extensions: VideoBrowsingContextExtensionsField
+    extensions: VideoBrowsingContextExtensions
 
 
-class VideoEnableClosedCaptioningContextField(BaseVideoContextField):
-    """Pydantic modle for video enable closed captioning `context` field.
+class VideoEnableClosedCaptioningContext(BaseVideoContext):
+    """Pydantic model for video enable closed captioning `context` property.
 
     Attributes:
-        extensions (dict): See VideoEnableClosedCaptioningContextExtensionsField.
+        extensions (dict): See VideoEnableClosedCaptioningContextExtensions.
     """
 
-    extensions: VideoEnableClosedCaptioningContextExtensionsField
+    extensions: VideoEnableClosedCaptioningContextExtensions
 
 
-class VideoVolumeChangeInteractionContextField(BaseVideoContextField):
-    """Pydantic model for video volume change interaction `context` field.
+class VideoVolumeChangeInteractionContext(BaseVideoContext):
+    """Pydantic model for video volume change interaction `context` property.
 
     Attributes:
-        extensions (dict): See VideoVolumeChangeInteractionContextExtensionsField.
+        extensions (dict): See VideoVolumeChangeInteractionContextExtensions.
     """
 
-    extensions: VideoVolumeChangeInteractionContextExtensionsField
+    extensions: VideoVolumeChangeInteractionContextExtensions
 
 
-class VideoScreenChangeInteractionContextField(BaseVideoContextField):
-    """Pydantic model for video screen change interaction `context` field.
+class VideoScreenChangeInteractionContext(BaseVideoContext):
+    """Pydantic model for video screen change interaction `context` property.
 
     Attributes:
-        extensions (dict): See VideoScreenChangeInteractionContextExtensionsField.
+        extensions (dict): See VideoScreenChangeInteractionContextExtensions.
     """
 
-    extensions: VideoScreenChangeInteractionContextExtensionsField
+    extensions: VideoScreenChangeInteractionContextExtensions
```

### Comparing `ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/results.py` & `ralph-malph-3.7.0/src/ralph/models/xapi/video/results.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,170 +6,170 @@
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from pydantic import Field, NonNegativeFloat
 
-from ...config import BaseExtensionModelWithConfig
-from ...fields.results import ResultField
-from ..constants import (
-    VIDEO_EXTENSION_CC_ENABLED,
-    VIDEO_EXTENSION_PLAYED_SEGMENTS,
-    VIDEO_EXTENSION_PROGRESS,
-    VIDEO_EXTENSION_TIME,
-    VIDEO_EXTENSION_TIME_FROM,
-    VIDEO_EXTENSION_TIME_TO,
+from ..base.results import BaseXapiResult
+from ..concepts.constants.video import (
+    CONTEXT_EXTENSION_CC_ENABLED,
+    CONTEXT_EXTENSION_PLAYED_SEGMENTS,
+    RESULT_EXTENSION_PROGRESS,
+    RESULT_EXTENSION_TIME,
+    RESULT_EXTENSION_TIME_FROM,
+    RESULT_EXTENSION_TIME_TO,
 )
+from ..config import BaseExtensionModelWithConfig
 
 
-class VideoResultExtensionsField(BaseExtensionModelWithConfig):
-    """Pydantic model for video `result`.`extensions` field.
+class VideoResultExtensions(BaseExtensionModelWithConfig):
+    """Pydantic model for video `result`.`extensions` property.
 
     Attributes:
         playedSegments (str): Consists of parts of the video the actor watched during
             current registration in chronological order (for example,
             "0[.]5[,]12[.]22[,]15[.]55[,]55[.]99.33[,]99.33").
         time (float): Consists of the video time code when the event was emitted.
     """
 
-    time: NonNegativeFloat = Field(alias=VIDEO_EXTENSION_TIME)
-    playedSegments: Optional[str] = Field(alias=VIDEO_EXTENSION_PLAYED_SEGMENTS)
+    time: NonNegativeFloat = Field(alias=RESULT_EXTENSION_TIME)
+    playedSegments: Optional[str] = Field(alias=CONTEXT_EXTENSION_PLAYED_SEGMENTS)
 
 
-class VideoPausedResultExtensionsField(VideoResultExtensionsField):
-    """Pydantic model for video paused `result`.`extensions` field.
+class VideoPausedResultExtensions(VideoResultExtensions):
+    """Pydantic model for video paused `result`.`extensions` property.
 
     Attributes:
         progress (float): Consists of the ratio of media consumed by the actor.
     """
 
-    progress: Optional[NonNegativeFloat] = Field(alias=VIDEO_EXTENSION_PROGRESS)
+    progress: Optional[NonNegativeFloat] = Field(alias=RESULT_EXTENSION_PROGRESS)
 
 
-class VideoSeekedResultExtensionsField(BaseExtensionModelWithConfig):
-    """Pydantic model for video seeked `result`.`extensions` field.
+class VideoSeekedResultExtensions(BaseExtensionModelWithConfig):
+    """Pydantic model for video seeked `result`.`extensions` property.
 
     Attributes:
         timeFrom (float): Consists of the point in time the actor changed from in a
             media object during a seek operation.
         timeTo (float): Consists of the point in time the actor changed to in a media
             object during a seek operation.
     """
 
-    timeFrom: NonNegativeFloat = Field(alias=VIDEO_EXTENSION_TIME_FROM)
-    timeTo: NonNegativeFloat = Field(alias=VIDEO_EXTENSION_TIME_TO)
+    timeFrom: NonNegativeFloat = Field(alias=RESULT_EXTENSION_TIME_FROM)
+    timeTo: NonNegativeFloat = Field(alias=RESULT_EXTENSION_TIME_TO)
 
 
-class VideoCompletedResultExtensionsField(VideoResultExtensionsField):
-    """Pydantic model for video completed `result`.`extensions` field.
+class VideoCompletedResultExtensions(VideoResultExtensions):
+    """Pydantic model for video completed `result`.`extensions` property.
 
     Attributes:
         progress (float): Consists of the percentage of media consumed by the actor.
     """
 
-    progress: NonNegativeFloat = Field(alias=VIDEO_EXTENSION_PROGRESS)
+    progress: NonNegativeFloat = Field(alias=RESULT_EXTENSION_PROGRESS)
 
 
-class VideoTerminatedResultExtensionsField(VideoResultExtensionsField):
-    """Pydantic model for video terminated `result`.`extensions` field.
+class VideoTerminatedResultExtensions(VideoResultExtensions):
+    """Pydantic model for video terminated `result`.`extensions` property.
 
     Attributes:
         progress (float): Consists of the percentage of media consumed by the actor.
     """
 
-    progress: NonNegativeFloat = Field(alias=VIDEO_EXTENSION_PROGRESS)
+    progress: NonNegativeFloat = Field(alias=RESULT_EXTENSION_PROGRESS)
 
 
-class VideoEnableClosedCaptioningResultExtensionsField(VideoResultExtensionsField):
-    """Pydantic model for video enable closed captioning `result`.`extensions` field.
+class VideoEnableClosedCaptioningResultExtensions(VideoResultExtensions):
+    """Pydantic model for video enable closed captioning `result`.`extensions` property.
 
     Attributes:
         ccEnabled (bool): Indicates whether subtitles are enabled.
     """
 
-    ccEnabled: bool = Field(alias=VIDEO_EXTENSION_CC_ENABLED)
+    ccEnabled: bool = Field(alias=CONTEXT_EXTENSION_CC_ENABLED)
 
 
-class VideoPlayedResultField(ResultField):
-    """Pydantic model for video played `result` field.
+class VideoPlayedResult(BaseXapiResult):
+    """Pydantic model for video played `result` property.
 
     Attributes:
-        extensions (dict): See VideoResultExtensionsField.
+        extensions (dict): See VideoResultExtensions.
     """
 
-    extensions: VideoResultExtensionsField
+    extensions: VideoResultExtensions
 
 
-class VideoPausedResultField(ResultField):
-    """Pydantic model for video paused `result` field.
+class VideoPausedResult(BaseXapiResult):
+    """Pydantic model for video paused `result` property.
 
     Attributes:
-        extensions (dict): See VideoPausedResultExtensionsField.
+        extensions (dict): See VideoPausedResultExtensions.
     """
 
-    extensions: VideoPausedResultExtensionsField
+    extensions: VideoPausedResultExtensions
 
 
-class VideoSeekedResultField(ResultField):
-    """Pydantic model for video seeked `result` field.
+class VideoSeekedResult(BaseXapiResult):
+    """Pydantic model for video seeked `result` property.
 
     Attributes:
-        extensions (dict): See VideoSeekedResultExtensionsField.
+        extensions (dict): See VideoSeekedResultExtensions.
     """
 
-    extensions: VideoSeekedResultExtensionsField
+    extensions: VideoSeekedResultExtensions
 
 
-class VideoCompletedResultField(ResultField):
-    """Pydantic model for video completed `result` field.
+class VideoCompletedResult(BaseXapiResult):
+    """Pydantic model for video completed `result` property.
 
     Attributes:
-        extensions (dict): See VideoCompletedResultExtensionsField.
+        extensions (dict): See VideoCompletedResultExtensions.
         completion (bool): Consists of the value `True`.
         duration (str): Consists of the total time spent consuming the video under
             current registration.
     """
 
-    extensions: VideoCompletedResultExtensionsField
+    extensions: VideoCompletedResultExtensions
     completion: Optional[Literal[True]]
     duration: Optional[timedelta]
 
 
-class VideoTerminatedResultField(ResultField):
-    """Pydantic model for video terminated `result` field.
+class VideoTerminatedResult(BaseXapiResult):
+    """Pydantic model for video terminated `result` property.
 
     Attributes:
-        extensions (dict): See VideoTerminatedResultExtensionsField.
+        extensions (dict): See VideoTerminatedResultExtensions.
     """
 
-    extensions: VideoTerminatedResultExtensionsField
+    extensions: VideoTerminatedResultExtensions
 
 
-class VideoEnableClosedCaptioningResultField(ResultField):
-    """Pydantic model for video enable closed captioning `result` field.
+class VideoEnableClosedCaptioningResult(BaseXapiResult):
+    """Pydantic model for video enable closed captioning `result` property.
 
     Attributes:
-        extensions (dict): See VideoEnableClosedCaptioningResultExtensionsField.
+        extensions (dict): See VideoEnableClosedCaptioningResultExtensions.
     """
 
-    extensions: VideoEnableClosedCaptioningResultExtensionsField
+    extensions: VideoEnableClosedCaptioningResultExtensions
 
 
-class VideoVolumeChangeInteractionResultField(ResultField):
-    """Pydantic model for video volume change interaction `result` field.
+class VideoVolumeChangeInteractionResult(BaseXapiResult):
+    """Pydantic model for video volume change interaction `result` property.
 
     Attributes:
-        extensions (dict): See VideoResultExtensionsField.
+        extensions (dict): See VideoResultExtensions.
     """
 
-    extensions: VideoResultExtensionsField
+    extensions: VideoResultExtensions
 
 
-class VideoScreenChangeInteractionResultField(ResultField):
-    """Pydantic model for video screen change interaction `result` field.
+class VideoScreenChangeInteractionResult(BaseXapiResult):
+    """Pydantic model for video screen change interaction `result` property.
 
     Attributes:
-        extensions (dict): See VideoResultExtensionsField.
+        extensions (dict): See VideoResultExtensions.
     """
 
-    extensions: VideoResultExtensionsField
+    extensions: VideoResultExtensions
```

### Comparing `ralph-malph-3.6.0/src/ralph/models/xapi/video/statements.py` & `ralph-malph-3.7.0/src/ralph/models/xapi/video/statements.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,235 +1,233 @@
 """Video xAPI event definitions."""
 
 from typing import Optional
 
 from ...selector import selector
-from ..base import BaseXapiModel
-from .fields.contexts import (
-    VideoCompletedContextField,
-    VideoEnableClosedCaptioningContextField,
-    VideoInitializedContextField,
-    VideoPausedContextField,
-    VideoPlayedContextField,
-    VideoScreenChangeInteractionContextField,
-    VideoSeekedContextField,
-    VideoTerminatedContextField,
-    VideoVolumeChangeInteractionContextField,
+from ..base.statements import BaseXapiStatement
+from ..concepts.activity_types.video import VideoActivity
+from ..concepts.verbs.scorm_profile import (
+    CompletedVerb,
+    InitializedVerb,
+    InteractedVerb,
+    TerminatedVerb,
 )
-from .fields.objects import VideoObjectField
-from .fields.results import (
-    VideoCompletedResultField,
-    VideoEnableClosedCaptioningResultField,
-    VideoPausedResultField,
-    VideoPlayedResultField,
-    VideoScreenChangeInteractionResultField,
-    VideoSeekedResultField,
-    VideoTerminatedResultField,
-    VideoVolumeChangeInteractionResultField,
+from ..concepts.verbs.video import PausedVerb, PlayedVerb, SeekedVerb
+from .contexts import (
+    VideoCompletedContext,
+    VideoEnableClosedCaptioningContext,
+    VideoInitializedContext,
+    VideoPausedContext,
+    VideoPlayedContext,
+    VideoScreenChangeInteractionContext,
+    VideoSeekedContext,
+    VideoTerminatedContext,
+    VideoVolumeChangeInteractionContext,
 )
-from .fields.verbs import (
-    VideoCompletedVerbField,
-    VideoInitializedVerbField,
-    VideoInteractedVerbField,
-    VideoPausedVerbField,
-    VideoPlayedVerbField,
-    VideoSeekedVerbField,
-    VideoTerminatedVerbField,
+from .results import (
+    VideoCompletedResult,
+    VideoEnableClosedCaptioningResult,
+    VideoPausedResult,
+    VideoPlayedResult,
+    VideoScreenChangeInteractionResult,
+    VideoSeekedResult,
+    VideoTerminatedResult,
+    VideoVolumeChangeInteractionResult,
 )
 
 
-class BaseVideoStatement(BaseXapiModel):
+class BaseVideoStatement(BaseXapiStatement):
     """Pydantic model for video core statements.
 
     Attributes:
-        object (dict): See VideoObjectField.
+        object (dict): See VideoActivity.
     """
 
-    object: VideoObjectField
+    object: VideoActivity
 
 
 class VideoInitialized(BaseVideoStatement):
     """Pydantic model for video initialized statement.
 
     Example: A video has been fully initialized.
 
     Attributes:
-        verb (dict): See VideoInitializedVerbField.
-        context (dict): See VideoInitializedContextField.
+        verb (dict): See InitializedVerb.
+        context (dict): See VideoInitializedContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="http://adlnet.gov/expapi/verbs/initialized",
     )
 
-    verb: VideoInitializedVerbField = VideoInitializedVerbField()
-    context: VideoInitializedContextField
+    verb: InitializedVerb = InitializedVerb()
+    context: VideoInitializedContext
 
 
 class VideoPlayed(BaseVideoStatement):
     """Pydantic model for video played statement.
 
     Example: John played the video or clicked the play button.
 
     Attributes:
-        verb (dict): See VideoPlayedVerbField.
-        result (dict): See VideoPlayedResultField.
-        context (dict): See VideoPlayedContextField.
+        verb (dict): See PlayedVerb.
+        result (dict): See VideoPlayedResult.
+        context (dict): See VideoPlayedContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="https://w3id.org/xapi/video/verbs/played",
     )
 
-    verb: VideoPlayedVerbField = VideoPlayedVerbField()
-    result: VideoPlayedResultField
-    context: Optional[VideoPlayedContextField]
+    verb: PlayedVerb = PlayedVerb()
+    result: VideoPlayedResult
+    context: Optional[VideoPlayedContext]
 
 
 class VideoPaused(BaseVideoStatement):
     """Pydantic model for video paused statement.
 
     Example: John paused the video or clicked the pause button.
 
     Attributes:
-        verb (dict): See VideoPausedVerbField.
-        result (dict): See VideoPausedResultField.
-        context (dict): See VideoPausedContextField.
+        verb (dict): See PausedVerb.
+        result (dict): See VideoPausedResult.
+        context (dict): See VideoPausedContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="https://w3id.org/xapi/video/verbs/paused",
     )
 
-    verb: VideoPausedVerbField = VideoPausedVerbField()
-    result: VideoPausedResultField
-    context: VideoPausedContextField
+    verb: PausedVerb = PausedVerb()
+    result: VideoPausedResult
+    context: VideoPausedContext
 
 
 class VideoSeeked(BaseVideoStatement):
     """Pydantic model for video seeked statement.
 
     Example: John moved the progress bar forward or backward to a specific time in the
         video.
 
     Attributes:
-        verb (dict): See VideoSeekedVerbField.
-        result (dict): See VideoSeekedResultField.
-        context (dict): See VideoSeekedContextField.
+        verb (dict): See SeekedVerb.
+        result (dict): See VideoSeekedResult.
+        context (dict): See VideoSeekedContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="https://w3id.org/xapi/video/verbs/seeked",
     )
 
-    verb: VideoSeekedVerbField = VideoSeekedVerbField()
-    result: VideoSeekedResultField
-    context: Optional[VideoSeekedContextField]
+    verb: SeekedVerb = SeekedVerb()
+    result: VideoSeekedResult
+    context: Optional[VideoSeekedContext]
 
 
 class VideoCompleted(BaseVideoStatement):
     """Pydantic model for video completed statement.
 
     Example: John completed a video by watching major parts of the video at least once.
 
     Attributes:
-        verb (dict): See VideoCompletedVerbField.
-        result (dict): See VideoCompletedResultField.
-        context (dict): See VideoCompletedContextField.
+        verb (dict): See CompletedVerb.
+        result (dict): See VideoCompletedResult.
+        context (dict): See VideoCompletedContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="http://adlnet.gov/expapi/verbs/completed",
     )
 
-    verb: VideoCompletedVerbField = VideoCompletedVerbField()
-    result: VideoCompletedResultField
-    context: VideoCompletedContextField
+    verb: CompletedVerb = CompletedVerb()
+    result: VideoCompletedResult
+    context: VideoCompletedContext
 
 
 class VideoTerminated(BaseVideoStatement):
     """Pydantic model for video terminated statement.
 
     Example: John ended a video (quit the player).
 
     Attributes:
-        verb (dict): See VideoTerminatedVerbField.
-        result (dict): See VideoTerminatedResultField.
-        context (dict): See VideoTerminatedContextField.
+        verb (dict): See TerminatedVerb.
+        result (dict): See VideoTerminatedResult.
+        context (dict): See VideoTerminatedContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="http://adlnet.gov/expapi/verbs/terminated",
     )
 
-    verb: VideoTerminatedVerbField = VideoTerminatedVerbField()
-    result: VideoTerminatedResultField
-    context: VideoTerminatedContextField
+    verb: TerminatedVerb = TerminatedVerb()
+    result: VideoTerminatedResult
+    context: VideoTerminatedContext
 
 
 class VideoEnableClosedCaptioning(BaseVideoStatement):
     """Pydantic model for video enable closed captioning statement.
 
     Example: John interacted with the player to enable closed captioning.
 
     Attributes:
-        verb (dict): See VideoInteractedVerbField.
-        result (dict): See VideoEnableClosedCaptioningResultField.
-        context (dict): See VideoEnableClosedCaptioningContextField.
+        verb (dict): See InteractedVerb.
+        result (dict): See VideoEnableClosedCaptioningResult.
+        context (dict): See VideoEnableClosedCaptioningContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="http://adlnet.gov/expapi/verbs/interacted",
     )
 
-    verb: VideoInteractedVerbField = VideoInteractedVerbField()
-    result: VideoEnableClosedCaptioningResultField
-    context: VideoEnableClosedCaptioningContextField
+    verb: InteractedVerb = InteractedVerb()
+    result: VideoEnableClosedCaptioningResult
+    context: VideoEnableClosedCaptioningContext
 
 
 class VideoVolumeChangeInteraction(BaseVideoStatement):
     """Pydantic model for video volume change interaction statement.
 
     Example: John interacted with the player to change the volume.
 
-    Attributes:
-        verb (dict): See VideoInteractedVerbField.
-        result (dict): See VideoVolumeChangeInteractionResultField.
-        context (dict): See VideoVolumeChangeInteractionContextField.
+    Attributes :
+        verb (dict): See InteractedVerb.
+        result (dict): See VideoVolumeChangeInteractionResult.
+        context (dict): See VideoVolumeChangeInteractionContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="http://adlnet.gov/expapi/verbs/interacted",
     )
 
-    verb: VideoInteractedVerbField = VideoInteractedVerbField()
-    result: VideoVolumeChangeInteractionResultField
-    context: VideoVolumeChangeInteractionContextField
+    verb: InteractedVerb = InteractedVerb()
+    result: VideoVolumeChangeInteractionResult
+    context: VideoVolumeChangeInteractionContext
 
 
 class VideoScreenChangeInteraction(BaseVideoStatement):
     """Pydantic model for video screen change interaction statement.
 
     Example: John interacted with the player to activate or deactivate full screen.
 
     Attributes:
-        verb (dict): See VideoInteractedVerbField.
-        result (dict): See VideoScreenChangeInteractionResultField.
-        context (dict): See VideoScreenChangeInteractionContextField.
+        verb (dict): See InteractedVerb.
+        result (dict): See VideoScreenChangeInteractionResult.
+        context (dict): See VideoScreenChangeInteractionContext.
     """
 
     __selector__ = selector(
         object__definition__type="https://w3id.org/xapi/video/activity-type/video",
         verb__id="http://adlnet.gov/expapi/verbs/interacted",
     )
 
-    verb: VideoInteractedVerbField = VideoInteractedVerbField()
-    result: VideoScreenChangeInteractionResultField
-    context: VideoScreenChangeInteractionContextField
+    verb: InteractedVerb = InteractedVerb()
+    result: VideoScreenChangeInteractionResult
+    context: VideoScreenChangeInteractionContext
```

### Comparing `ralph-malph-3.6.0/src/ralph/parsers.py` & `ralph-malph-3.7.0/src/ralph/parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph/utils.py` & `ralph-malph-3.7.0/src/ralph/utils.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/src/ralph_malph.egg-info/PKG-INFO` & `ralph-malph-3.7.0/src/ralph_malph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.6.0
+Version: 3.7.0
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: backend-clickhouse
 Provides-Extra: backend-es
 Provides-Extra: backend-ldp
+Provides-Extra: backend-lrs
 Provides-Extra: backend-mongo
 Provides-Extra: backend-s3
 Provides-Extra: backend-swift
 Provides-Extra: backend-ws
 Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: ci
```

### Comparing `ralph-malph-3.6.0/src/ralph_malph.egg-info/requires.txt` & `ralph-malph-3.7.0/src/ralph_malph.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 [backend-es]
 elasticsearch>=8.0.0
 
 [backend-ldp]
 ovh>=1.0.0
 requests>=2.0.0
 
+[backend-lrs]
+httpx==0.24.1
+more-itertools==9.1.0
+
 [backend-mongo]
 pymongo[srv]>=4.0.0
 python-dateutil>=2.8.2
 
 [backend-s3]
 boto3>=1.24.70
 botocore>=1.27.71
@@ -36,31 +40,36 @@
 click>=8.1.0
 click-option-group>=0.5.0
 sentry-sdk[fastapi]>=1.9.0
 
 [dev]
 bandit==1.7.5
 black==23.3.0
+cryptography==40.0.1
 factory-boy==3.2.1
 flake8==6.0.0
-hypothesis==6.75.3
+hypothesis==6.78.1
 isort==5.12.0
 logging-gelf==0.0.26
 mkdocs==1.4.3
 mkdocs-click==0.8.0
-mkdocs-material==9.1.12
-mkdocstrings[python-legacy]==0.21.2
-moto==4.1.9
+mkdocs-material==9.1.15
+mkdocstrings[python-legacy]==0.22.0
+moto==4.1.11
 pydocstyle==6.3.0
 pyfakefs==5.2.2
 pylint==2.17.4
-pytest==7.3.1
+pytest==7.3.2
 pytest-asyncio==0.21.0
-pytest-cov==4.0.0
+pytest-cov==4.1.0
+pytest-httpx==0.22.0
+responses==0.23.1
 
 [lrs]
 bcrypt==4.0.1
-fastapi==0.95.1
+fastapi==0.97.0
+cachetools==5.3.1
 h11>=0.11.0
-httpx==0.24.0
-sentry_sdk==1.22.2
+httpx==0.24.1
+sentry_sdk==1.25.1
+python-jose==3.3.0
 uvicorn[standard]==0.22.0
```

### Comparing `ralph-malph-3.6.0/tests/test_cli.py` & `ralph-malph-3.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/tests/test_cli_usage.py` & `ralph-malph-3.7.0/tests/test_cli_usage.py`

 * *Files 14% similar despite different names*

```diff
@@ -101,19 +101,20 @@
     """Tests ralph fetch command usage."""
     runner = CliRunner()
     result = runner.invoke(cli, ["fetch", "--help"])
 
     assert result.exit_code == 0
     assert (
         "Options:\n"
-        "  -b, --backend [es|mongo|clickhouse|ldp|fs|swift|s3|ws]\n"
+        "  -b, --backend [es|mongo|clickhouse|lrs|ldp|fs|swift|s3|ws]\n"
         "                                  Backend  [required]\n"
         "  ws backend: \n"
         "    --ws-uri TEXT\n"
         "  s3 backend: \n"
+        "    --s3-endpoint-url TEXT\n"
         "    --s3-bucket-name TEXT\n"
         "    --s3-default-region TEXT\n"
         "    --s3-session-token TEXT\n"
         "    --s3-secret-access-key TEXT\n"
         "    --s3-access-key-id TEXT\n"
         "  swift backend: \n"
         "    --swift-os-identity-api-version TEXT\n"
@@ -131,14 +132,21 @@
         "  ldp backend: \n"
         "    --ldp-stream-id TEXT\n"
         "    --ldp-service-name TEXT\n"
         "    --ldp-consumer-key TEXT\n"
         "    --ldp-application-secret TEXT\n"
         "    --ldp-application-key TEXT\n"
         "    --ldp-endpoint TEXT\n"
+        "  lrs backend: \n"
+        "    --lrs-statements-endpoint TEXT\n"
+        "    --lrs-status-endpoint TEXT\n"
+        "    --lrs-headers KEY=VALUE,KEY=VALUE\n"
+        "    --lrs-password TEXT\n"
+        "    --lrs-username TEXT\n"
+        "    --lrs-base-url TEXT\n"
         "  clickhouse backend: \n"
         "    --clickhouse-client-options KEY=VALUE,KEY=VALUE\n"
         "    --clickhouse-password TEXT\n"
         "    --clickhouse-username TEXT\n"
         "    --clickhouse-event-table-name TEXT\n"
         "    --clickhouse-database TEXT\n"
         "    --clickhouse-port INTEGER\n"
@@ -150,39 +158,42 @@
         "    --mongo-connection-uri TEXT\n"
         "  es backend: \n"
         "    --es-op-type TEXT\n"
         "    --es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --es-index TEXT\n"
         "    --es-hosts VALUE1,VALUE2,VALUE3\n"
         "  -c, --chunk-size INTEGER        Get events by chunks of size #\n"
+        "  -t, --target TEXT               Endpoint from which to fetch events (e.g.\n"
+        "                                  `/statements`)\n"
         '  -q, --query \'{"KEY": "VALUE", "KEY": "VALUE"}\'\n'
         "                                  Query object as a JSON string (database\n"
         "                                  backends ONLY)\n"
     ) in result.output
     logging.warning(result.output)
     result = runner.invoke(cli, ["fetch"])
     assert result.exit_code > 0
     assert (
         "Error: Missing option '-b' / '--backend'. "
-        "Choose from:\n\tes,\n\tmongo,\n\tclickhouse,\n\tldp,\n\tfs,\n\tswift,\n\ts3,"
-        "\n\tws\n"
+        "Choose from:\n\tes,\n\tmongo,\n\tclickhouse,\n\tlrs,\n\tldp,\n\tfs,\n\tswift,"
+        "\n\ts3,\n\tws\n"
     ) in result.output
 
 
 def test_cli_list_command_usage():
     """Tests ralph list command usage."""
     runner = CliRunner()
     result = runner.invoke(cli, ["list", "--help"])
 
     assert result.exit_code == 0
     assert (
         "Options:\n"
         "  -b, --backend [ldp|fs|swift|s3]\n"
         "                                  Backend  [required]\n"
         "  s3 backend: \n"
+        "    --s3-endpoint-url TEXT\n"
         "    --s3-bucket-name TEXT\n"
         "    --s3-default-region TEXT\n"
         "    --s3-session-token TEXT\n"
         "    --s3-secret-access-key TEXT\n"
         "    --s3-access-key-id TEXT\n"
         "  swift backend: \n"
         "    --swift-os-identity-api-version TEXT\n"
```

### Comparing `ralph-malph-3.6.0/tests/test_conf.py` & `ralph-malph-3.7.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/tests/test_dependencies.py` & `ralph-malph-3.7.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/tests/test_filters.py` & `ralph-malph-3.7.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/tests/test_logger.py` & `ralph-malph-3.7.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/tests/test_parsers.py` & `ralph-malph-3.7.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.6.0/tests/test_utils.py` & `ralph-malph-3.7.0/tests/test_utils.py`

 * *Files identical despite different names*

