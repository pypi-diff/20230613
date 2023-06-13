# Comparing `tmp/scarletio-1.0.8.tar.gz` & `tmp/scarletio-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarletio-1.0.8.tar", last modified: Tue Jan  4 19:46:29 2022, max compression
+gzip compressed data, was "scarletio-1.0.9.tar", last modified: Tue Jan 25 21:12:56 2022, max compression
```

## Comparing `scarletio-1.0.8.tar` & `scarletio-1.0.9.tar`

### file list

```diff
@@ -1,130 +1,132 @@
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.978285 scarletio-1.0.8/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1137 2022-01-04 19:46:29.978285 scarletio-1.0.8/PKG-INFO
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2021-12-01 08:05:48.000000 scarletio-1.0.8/README.md
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.954285 scarletio-1.0.8/scarletio/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      193 2022-01-04 19:45:52.000000 scarletio-1.0.8/scarletio/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.954285 scarletio-1.0.8/scarletio/core/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      413 2021-12-03 22:31:24.000000 scarletio-1.0.8/scarletio/core/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.958285 scarletio-1.0.8/scarletio/core/event_loop/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      526 2021-12-02 17:55:18.000000 scarletio-1.0.8/scarletio/core/event_loop/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17607 2022-01-01 17:24:17.000000 scarletio-1.0.8/scarletio/core/event_loop/cycler.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   122099 2022-01-04 17:44:08.000000 scarletio-1.0.8/scarletio/core/event_loop/event_loop.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7354 2022-01-01 17:46:45.000000 scarletio-1.0.8/scarletio/core/event_loop/event_loop_functionality_helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2312 2021-12-02 06:29:44.000000 scarletio-1.0.8/scarletio/core/event_loop/event_thread_suspender.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5589 2022-01-01 18:48:38.000000 scarletio-1.0.8/scarletio/core/event_loop/event_thread_type.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28438 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/core/event_loop/executor.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9634 2022-01-01 18:51:59.000000 scarletio-1.0.8/scarletio/core/event_loop/handles.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7422 2022-01-01 18:52:15.000000 scarletio-1.0.8/scarletio/core/event_loop/selector.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5153 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/core/event_loop/server.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2040 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/core/exceptions.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    41155 2022-01-01 18:55:41.000000 scarletio-1.0.8/scarletio/core/ios.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.958285 scarletio-1.0.8/scarletio/core/protocols_and_transports/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      418 2021-12-02 18:06:20.000000 scarletio-1.0.8/scarletio/core/protocols_and_transports/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12767 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/core/protocols_and_transports/abstract.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3829 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/core/protocols_and_transports/extra_info.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    35140 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/core/protocols_and_transports/protocol.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14344 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/core/protocols_and_transports/ssl_pipe.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17681 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/core/protocols_and_transports/ssl_transport_layer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    31011 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/core/protocols_and_transports/transport_layer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21047 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/core/protocols_and_transports/unix_pipe_transport_layer.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.958285 scarletio-1.0.8/scarletio/core/subprocess/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      202 2021-12-02 18:03:33.000000 scarletio-1.0.8/scarletio/core/subprocess/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    30286 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/core/subprocess/subprocess.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3089 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/core/subprocess/subprocess_protocols.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2621 2022-01-01 18:55:21.000000 scarletio-1.0.8/scarletio/core/subprocess/subprocess_writer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      186 2022-01-01 18:55:45.000000 scarletio-1.0.8/scarletio/core/time.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5518 2022-01-01 18:56:00.000000 scarletio-1.0.8/scarletio/core/top_level.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.962285 scarletio-1.0.8/scarletio/core/traps/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1108 2021-12-02 18:10:27.000000 scarletio-1.0.8/scarletio/core/traps/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18352 2022-01-03 19:53:06.000000 scarletio-1.0.8/scarletio/core/traps/async_executing.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2475 2022-01-03 19:53:24.000000 scarletio-1.0.8/scarletio/core/traps/event.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20168 2022-01-03 19:53:39.000000 scarletio-1.0.8/scarletio/core/traps/future.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15244 2022-01-03 19:53:54.000000 scarletio-1.0.8/scarletio/core/traps/future_async_wrapper.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4840 2022-01-03 19:54:16.000000 scarletio-1.0.8/scarletio/core/traps/future_chaining.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19839 2022-01-03 19:54:27.000000 scarletio-1.0.8/scarletio/core/traps/future_sync_wrapper.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10483 2022-01-03 19:54:44.000000 scarletio-1.0.8/scarletio/core/traps/gatherer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3761 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/core/traps/handle_cancellers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7614 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/core/traps/locks.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16114 2022-01-03 19:55:05.000000 scarletio-1.0.8/scarletio/core/traps/queues.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6594 2022-01-03 19:55:30.000000 scarletio-1.0.8/scarletio/core/traps/result_gathering_future.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19245 2022-01-03 19:55:52.000000 scarletio-1.0.8/scarletio/core/traps/task.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1706 2022-01-03 19:56:09.000000 scarletio-1.0.8/scarletio/core/traps/task_suppression.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7311 2022-01-03 19:56:21.000000 scarletio-1.0.8/scarletio/core/traps/task_thread_switcher.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5266 2022-01-03 19:56:56.000000 scarletio-1.0.8/scarletio/core/traps/timeouting.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18650 2022-01-03 19:57:07.000000 scarletio-1.0.8/scarletio/core/traps/wait_continously.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5045 2022-01-03 19:57:21.000000 scarletio-1.0.8/scarletio/core/traps/wait_till_all.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5167 2022-01-03 19:57:21.000000 scarletio-1.0.8/scarletio/core/traps/wait_till_exception.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12095 2022-01-03 19:57:32.000000 scarletio-1.0.8/scarletio/core/traps/wait_till_first.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.966285 scarletio-1.0.8/scarletio/http_client/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      534 2021-12-02 06:29:44.000000 scarletio-1.0.8/scarletio/http_client/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13825 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/http_client/client_request.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13176 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/http_client/client_response.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5937 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/http_client/connection.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2881 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/http_client/connection_key.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    31885 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/http_client/connector.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2935 2022-01-01 18:59:55.000000 scarletio-1.0.8/scarletio/http_client/fingerprint.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    35727 2022-01-01 19:00:25.000000 scarletio-1.0.8/scarletio/http_client/http_client.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5556 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/http_client/request_context_managers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1021 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/http_client/request_info.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.970285 scarletio-1.0.8/scarletio/utils/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1710 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/utils/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    34437 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/utils/analyzer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7293 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/utils/async_utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3400 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/utils/base_method.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      319 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/utils/code.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      343 2021-12-01 08:05:48.000000 scarletio-1.0.8/scarletio/utils/compact.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2076 2021-12-31 07:40:01.000000 scarletio-1.0.8/scarletio/utils/dict_update_iterable_iterator.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2010 2022-01-01 19:02:15.000000 scarletio-1.0.8/scarletio/utils/docs.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2009 2022-01-01 19:02:30.000000 scarletio-1.0.8/scarletio/utils/export_include.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2615 2022-01-01 19:02:41.000000 scarletio-1.0.8/scarletio/utils/function_tools.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21513 2022-01-01 19:02:58.000000 scarletio-1.0.8/scarletio/utils/hybrid_value_dictionary.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7155 2022-01-01 19:03:12.000000 scarletio-1.0.8/scarletio/utils/ignore_case_multi_value_dictionary.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3332 2022-01-01 19:03:31.000000 scarletio-1.0.8/scarletio/utils/ignore_case_string.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1088 2022-01-01 19:03:42.000000 scarletio-1.0.8/scarletio/utils/json.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2874 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/utils/keep_type.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2166 2022-01-01 19:03:53.000000 scarletio-1.0.8/scarletio/utils/method_like.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12289 2022-01-01 19:03:58.000000 scarletio-1.0.8/scarletio/utils/multi_value_dictionary.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7897 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/utils/properties.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1420 2022-01-01 19:04:06.000000 scarletio-1.0.8/scarletio/utils/removed_descriptor.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4583 2022-01-01 19:04:11.000000 scarletio-1.0.8/scarletio/utils/rich_attribute_error.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11083 2022-01-01 19:04:16.000000 scarletio-1.0.8/scarletio/utils/sorted_list.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14932 2022-01-01 19:06:51.000000 scarletio-1.0.8/scarletio/utils/trace.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      983 2022-01-01 19:07:07.000000 scarletio-1.0.8/scarletio/utils/type_methodizer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5470 2022-01-01 19:07:32.000000 scarletio-1.0.8/scarletio/utils/type_modulizer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7885 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/utils/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8551 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/utils/weak_core.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20828 2022-01-01 19:08:39.000000 scarletio-1.0.8/scarletio/utils/weak_item_dictionary.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18781 2022-01-01 19:08:54.000000 scarletio-1.0.8/scarletio/utils/weak_key_dictionary.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12174 2022-01-01 19:09:09.000000 scarletio-1.0.8/scarletio/utils/weak_map.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20379 2022-01-01 19:09:25.000000 scarletio-1.0.8/scarletio/utils/weak_value_dictionary.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.974285 scarletio-1.0.8/scarletio/web_common/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      847 2021-12-02 06:29:44.000000 scarletio-1.0.8/scarletio/web_common/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2706 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/web_common/compressors.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12552 2022-01-01 19:09:53.000000 scarletio-1.0.8/scarletio/web_common/cookiejar.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6364 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/web_common/exceptions.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10093 2022-01-01 19:10:13.000000 scarletio-1.0.8/scarletio/web_common/formdata.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13239 2022-01-01 19:10:13.000000 scarletio-1.0.8/scarletio/web_common/header_building_and_parsing.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4472 2022-01-01 19:10:19.000000 scarletio-1.0.8/scarletio/web_common/headers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11763 2022-01-01 19:10:34.000000 scarletio-1.0.8/scarletio/web_common/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4745 2022-01-01 19:10:59.000000 scarletio-1.0.8/scarletio/web_common/http_message.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    47488 2022-01-01 19:11:13.000000 scarletio-1.0.8/scarletio/web_common/http_protocol.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5256 2022-01-01 19:11:30.000000 scarletio-1.0.8/scarletio/web_common/http_stream_writer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1603 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/web_common/mime_type.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    48139 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/web_common/multipart.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6213 2022-01-04 18:05:12.000000 scarletio-1.0.8/scarletio/web_common/quoting.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    41175 2022-01-01 19:12:30.000000 scarletio-1.0.8/scarletio/web_common/url.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6890 2022-01-01 19:12:34.000000 scarletio-1.0.8/scarletio/web_common/websocket_frame.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.978285 scarletio-1.0.8/scarletio/websocket/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      303 2021-12-02 06:29:44.000000 scarletio-1.0.8/scarletio/websocket/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17434 2022-01-01 19:12:52.000000 scarletio-1.0.8/scarletio/websocket/websocket_client.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    41369 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/websocket/websocket_common_protocol.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15928 2022-01-01 19:13:23.000000 scarletio-1.0.8/scarletio/websocket/websocket_server.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    24673 2022-01-03 06:21:53.000000 scarletio-1.0.8/scarletio/websocket/websocket_server_protocol.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-04 19:46:29.954285 scarletio-1.0.8/scarletio.egg-info/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1137 2022-01-04 19:46:29.000000 scarletio-1.0.8/scarletio.egg-info/PKG-INFO
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4322 2022-01-04 19:46:29.000000 scarletio-1.0.8/scarletio.egg-info/SOURCES.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        1 2022-01-04 19:46:29.000000 scarletio-1.0.8/scarletio.egg-info/dependency_links.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       46 2022-01-04 19:46:29.000000 scarletio-1.0.8/scarletio.egg-info/requires.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2022-01-04 19:46:29.000000 scarletio-1.0.8/scarletio.egg-info/top_level.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2022-01-04 19:46:29.978285 scarletio-1.0.8/setup.cfg
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2302 2022-01-01 19:14:03.000000 scarletio-1.0.8/setup.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.802413 scarletio-1.0.9/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2052 2022-01-25 21:12:56.802413 scarletio-1.0.9/PKG-INFO
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      769 2022-01-20 07:24:27.000000 scarletio-1.0.9/README.md
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.778413 scarletio-1.0.9/scarletio/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      193 2022-01-25 20:42:25.000000 scarletio-1.0.9/scarletio/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.778413 scarletio-1.0.9/scarletio/core/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      413 2021-12-03 22:31:24.000000 scarletio-1.0.9/scarletio/core/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.782413 scarletio-1.0.9/scarletio/core/event_loop/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      526 2021-12-02 17:55:18.000000 scarletio-1.0.9/scarletio/core/event_loop/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17607 2022-01-01 17:24:17.000000 scarletio-1.0.9/scarletio/core/event_loop/cycler.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   122099 2022-01-04 17:44:08.000000 scarletio-1.0.9/scarletio/core/event_loop/event_loop.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7354 2022-01-01 17:46:45.000000 scarletio-1.0.9/scarletio/core/event_loop/event_loop_functionality_helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2312 2021-12-02 06:29:44.000000 scarletio-1.0.9/scarletio/core/event_loop/event_thread_suspender.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5589 2022-01-01 18:48:38.000000 scarletio-1.0.9/scarletio/core/event_loop/event_thread_type.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28438 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/core/event_loop/executor.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9634 2022-01-01 18:51:59.000000 scarletio-1.0.9/scarletio/core/event_loop/handles.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7422 2022-01-01 18:52:15.000000 scarletio-1.0.9/scarletio/core/event_loop/selector.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5153 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/core/event_loop/server.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2040 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/core/exceptions.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    41155 2022-01-01 18:55:41.000000 scarletio-1.0.9/scarletio/core/ios.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.782413 scarletio-1.0.9/scarletio/core/protocols_and_transports/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      418 2021-12-02 18:06:20.000000 scarletio-1.0.9/scarletio/core/protocols_and_transports/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12767 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/core/protocols_and_transports/abstract.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3829 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/core/protocols_and_transports/extra_info.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    35140 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/core/protocols_and_transports/protocol.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14344 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/core/protocols_and_transports/ssl_pipe.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17681 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/core/protocols_and_transports/ssl_transport_layer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    31011 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/core/protocols_and_transports/transport_layer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21047 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/core/protocols_and_transports/unix_pipe_transport_layer.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.786413 scarletio-1.0.9/scarletio/core/subprocess/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      202 2021-12-02 18:03:33.000000 scarletio-1.0.9/scarletio/core/subprocess/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    30286 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/core/subprocess/subprocess.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3089 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/core/subprocess/subprocess_protocols.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2621 2022-01-01 18:55:21.000000 scarletio-1.0.9/scarletio/core/subprocess/subprocess_writer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      186 2022-01-01 18:55:45.000000 scarletio-1.0.9/scarletio/core/time.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5518 2022-01-01 18:56:00.000000 scarletio-1.0.9/scarletio/core/top_level.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.790413 scarletio-1.0.9/scarletio/core/traps/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1108 2021-12-02 18:10:27.000000 scarletio-1.0.9/scarletio/core/traps/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18352 2022-01-03 19:53:06.000000 scarletio-1.0.9/scarletio/core/traps/async_executing.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2475 2022-01-03 19:53:24.000000 scarletio-1.0.9/scarletio/core/traps/event.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20648 2022-01-18 14:47:22.000000 scarletio-1.0.9/scarletio/core/traps/future.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15244 2022-01-03 19:53:54.000000 scarletio-1.0.9/scarletio/core/traps/future_async_wrapper.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4840 2022-01-03 19:54:16.000000 scarletio-1.0.9/scarletio/core/traps/future_chaining.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19839 2022-01-03 19:54:27.000000 scarletio-1.0.9/scarletio/core/traps/future_sync_wrapper.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10483 2022-01-03 19:54:44.000000 scarletio-1.0.9/scarletio/core/traps/gatherer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3761 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/core/traps/handle_cancellers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7614 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/core/traps/locks.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16114 2022-01-03 19:55:05.000000 scarletio-1.0.9/scarletio/core/traps/queues.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6594 2022-01-03 19:55:30.000000 scarletio-1.0.9/scarletio/core/traps/result_gathering_future.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19245 2022-01-03 19:55:52.000000 scarletio-1.0.9/scarletio/core/traps/task.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1706 2022-01-03 19:56:09.000000 scarletio-1.0.9/scarletio/core/traps/task_suppression.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7311 2022-01-03 19:56:21.000000 scarletio-1.0.9/scarletio/core/traps/task_thread_switcher.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5266 2022-01-03 19:56:56.000000 scarletio-1.0.9/scarletio/core/traps/timeouting.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18650 2022-01-03 19:57:07.000000 scarletio-1.0.9/scarletio/core/traps/wait_continously.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5045 2022-01-03 19:57:21.000000 scarletio-1.0.9/scarletio/core/traps/wait_till_all.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5167 2022-01-03 19:57:21.000000 scarletio-1.0.9/scarletio/core/traps/wait_till_exception.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12095 2022-01-03 19:57:32.000000 scarletio-1.0.9/scarletio/core/traps/wait_till_first.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.790413 scarletio-1.0.9/scarletio/http_client/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      534 2021-12-02 06:29:44.000000 scarletio-1.0.9/scarletio/http_client/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13825 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/http_client/client_request.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13176 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/http_client/client_response.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5937 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/http_client/connection.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2881 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/http_client/connection_key.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    31885 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/http_client/connector.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2935 2022-01-01 18:59:55.000000 scarletio-1.0.9/scarletio/http_client/fingerprint.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    35727 2022-01-01 19:00:25.000000 scarletio-1.0.9/scarletio/http_client/http_client.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5556 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/http_client/request_context_managers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1021 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/http_client/request_info.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.798413 scarletio-1.0.9/scarletio/utils/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1826 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    34437 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/utils/analyzer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7293 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/utils/async_utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3400 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/utils/base_method.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      319 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/utils/code.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      343 2021-12-01 08:05:48.000000 scarletio-1.0.9/scarletio/utils/compact.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6263 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/dict_iterator_bases.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2076 2021-12-31 07:40:01.000000 scarletio-1.0.9/scarletio/utils/dict_update_iterable_iterator.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2010 2022-01-01 19:02:15.000000 scarletio-1.0.9/scarletio/utils/docs.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2009 2022-01-01 19:02:30.000000 scarletio-1.0.9/scarletio/utils/export_include.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2615 2022-01-01 19:02:41.000000 scarletio-1.0.9/scarletio/utils/function_tools.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20352 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/hybrid_value_dictionary.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3642 2022-01-25 20:07:35.000000 scarletio-1.0.9/scarletio/utils/ignore_case_multi_value_dictionary.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3332 2022-01-01 19:03:31.000000 scarletio-1.0.9/scarletio/utils/ignore_case_string.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1088 2022-01-01 19:03:42.000000 scarletio-1.0.9/scarletio/utils/json.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2874 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/utils/keep_type.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2166 2022-01-01 19:03:53.000000 scarletio-1.0.9/scarletio/utils/method_like.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12843 2022-01-25 20:07:35.000000 scarletio-1.0.9/scarletio/utils/multi_value_dictionary.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7897 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/utils/properties.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1420 2022-01-01 19:04:06.000000 scarletio-1.0.9/scarletio/utils/removed_descriptor.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4583 2022-01-01 19:04:11.000000 scarletio-1.0.9/scarletio/utils/rich_attribute_error.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11083 2022-01-01 19:04:16.000000 scarletio-1.0.9/scarletio/utils/sorted_list.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14932 2022-01-01 19:06:51.000000 scarletio-1.0.9/scarletio/utils/trace.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      983 2022-01-01 19:07:07.000000 scarletio-1.0.9/scarletio/utils/type_methodizer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5470 2022-01-01 19:07:32.000000 scarletio-1.0.9/scarletio/utils/type_modulizer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8684 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8910 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/weak_core.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20650 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/weak_item_dictionary.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17789 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/weak_key_dictionary.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13417 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/weak_map.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    31919 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/weak_set.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19242 2022-01-20 07:14:37.000000 scarletio-1.0.9/scarletio/utils/weak_value_dictionary.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.802413 scarletio-1.0.9/scarletio/web_common/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      847 2021-12-02 06:29:44.000000 scarletio-1.0.9/scarletio/web_common/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2706 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/web_common/compressors.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12552 2022-01-01 19:09:53.000000 scarletio-1.0.9/scarletio/web_common/cookiejar.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6364 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/web_common/exceptions.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10093 2022-01-01 19:10:13.000000 scarletio-1.0.9/scarletio/web_common/formdata.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13239 2022-01-01 19:10:13.000000 scarletio-1.0.9/scarletio/web_common/header_building_and_parsing.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4472 2022-01-01 19:10:19.000000 scarletio-1.0.9/scarletio/web_common/headers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11763 2022-01-01 19:10:34.000000 scarletio-1.0.9/scarletio/web_common/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4745 2022-01-01 19:10:59.000000 scarletio-1.0.9/scarletio/web_common/http_message.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    47488 2022-01-01 19:11:13.000000 scarletio-1.0.9/scarletio/web_common/http_protocol.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5256 2022-01-01 19:11:30.000000 scarletio-1.0.9/scarletio/web_common/http_stream_writer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1603 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/web_common/mime_type.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    48139 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/web_common/multipart.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6213 2022-01-04 18:05:12.000000 scarletio-1.0.9/scarletio/web_common/quoting.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    41175 2022-01-01 19:12:30.000000 scarletio-1.0.9/scarletio/web_common/url.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6890 2022-01-01 19:12:34.000000 scarletio-1.0.9/scarletio/web_common/websocket_frame.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.802413 scarletio-1.0.9/scarletio/websocket/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      303 2021-12-02 06:29:44.000000 scarletio-1.0.9/scarletio/websocket/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17434 2022-01-01 19:12:52.000000 scarletio-1.0.9/scarletio/websocket/websocket_client.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    41369 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/websocket/websocket_common_protocol.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15928 2022-01-01 19:13:23.000000 scarletio-1.0.9/scarletio/websocket/websocket_server.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    24673 2022-01-03 06:21:53.000000 scarletio-1.0.9/scarletio/websocket/websocket_server_protocol.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-01-25 21:12:56.778413 scarletio-1.0.9/scarletio.egg-info/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2052 2022-01-25 21:12:56.000000 scarletio-1.0.9/scarletio.egg-info/PKG-INFO
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4389 2022-01-25 21:12:56.000000 scarletio-1.0.9/scarletio.egg-info/SOURCES.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        1 2022-01-25 21:12:56.000000 scarletio-1.0.9/scarletio.egg-info/dependency_links.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       46 2022-01-25 21:12:56.000000 scarletio-1.0.9/scarletio.egg-info/requires.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2022-01-25 21:12:56.000000 scarletio-1.0.9/scarletio.egg-info/top_level.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2022-01-25 21:12:56.802413 scarletio-1.0.9/setup.cfg
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2302 2022-01-01 19:14:03.000000 scarletio-1.0.9/setup.py
```

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/__init__.py` & `scarletio-1.0.9/scarletio/core/event_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/cycler.py` & `scarletio-1.0.9/scarletio/core/event_loop/cycler.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/event_loop.py` & `scarletio-1.0.9/scarletio/core/event_loop/event_loop.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/event_loop_functionality_helpers.py` & `scarletio-1.0.9/scarletio/core/event_loop/event_loop_functionality_helpers.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/event_thread_suspender.py` & `scarletio-1.0.9/scarletio/core/event_loop/event_thread_suspender.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/event_thread_type.py` & `scarletio-1.0.9/scarletio/core/event_loop/event_thread_type.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/executor.py` & `scarletio-1.0.9/scarletio/core/event_loop/executor.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/handles.py` & `scarletio-1.0.9/scarletio/core/event_loop/handles.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/selector.py` & `scarletio-1.0.9/scarletio/core/event_loop/selector.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/event_loop/server.py` & `scarletio-1.0.9/scarletio/core/event_loop/server.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/exceptions.py` & `scarletio-1.0.9/scarletio/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/ios.py` & `scarletio-1.0.9/scarletio/core/ios.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/protocols_and_transports/abstract.py` & `scarletio-1.0.9/scarletio/core/protocols_and_transports/abstract.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/protocols_and_transports/extra_info.py` & `scarletio-1.0.9/scarletio/core/protocols_and_transports/extra_info.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/protocols_and_transports/protocol.py` & `scarletio-1.0.9/scarletio/core/protocols_and_transports/protocol.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/protocols_and_transports/ssl_pipe.py` & `scarletio-1.0.9/scarletio/core/protocols_and_transports/ssl_pipe.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/protocols_and_transports/ssl_transport_layer.py` & `scarletio-1.0.9/scarletio/core/protocols_and_transports/ssl_transport_layer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/protocols_and_transports/transport_layer.py` & `scarletio-1.0.9/scarletio/core/protocols_and_transports/transport_layer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/protocols_and_transports/unix_pipe_transport_layer.py` & `scarletio-1.0.9/scarletio/core/protocols_and_transports/unix_pipe_transport_layer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/subprocess/subprocess.py` & `scarletio-1.0.9/scarletio/core/subprocess/subprocess.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/subprocess/subprocess_protocols.py` & `scarletio-1.0.9/scarletio/core/subprocess/subprocess_protocols.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/subprocess/subprocess_writer.py` & `scarletio-1.0.9/scarletio/core/subprocess/subprocess_writer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/top_level.py` & `scarletio-1.0.9/scarletio/core/top_level.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/__init__.py` & `scarletio-1.0.9/scarletio/core/traps/__init__.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/async_executing.py` & `scarletio-1.0.9/scarletio/core/traps/async_executing.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/event.py` & `scarletio-1.0.9/scarletio/core/traps/event.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/future.py` & `scarletio-1.0.9/scarletio/core/traps/future.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __all__ = ('Future',)
 
 import reprlib, sys, warnings
 
-from ...utils import ignore_frame, include, set_docs
+from ...utils import ignore_frame, include, set_docs, to_coroutine
 from ...utils.trace import format_callback
 
 from ..exceptions import CancelledError, InvalidStateError
 
 from .handle_cancellers import _HandleCancellerBase
 
 
@@ -537,14 +537,31 @@
             self._blocking = True
             yield self
         
         return self.result()
     
     __await__ = __iter__
     
+    
+    @to_coroutine
+    def wait_for_completion(self):
+        """
+        Awaits the future till it is done, not retrieving it's result.
+        
+        This method is an awaitable generator.
+        
+        Notes
+        -----
+        This method do not protects the future from task cancellation, or from timeout context managers.
+        """
+        if self._state == FUTURE_STATE_PENDING:
+            self._blocking = True
+            yield self
+    
+    
     if __debug__:
         def __del__(self):
             """
             If the future is pending, but it's result was not set, meanwhile anything awaits at it, notifies it.
             
             Also notifies if the future's result was set with ``.set_exception``, or with
             ``.set_exception_if_pending``, and it was not retrieved.
```

### Comparing `scarletio-1.0.8/scarletio/core/traps/future_async_wrapper.py` & `scarletio-1.0.9/scarletio/core/traps/future_async_wrapper.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/future_chaining.py` & `scarletio-1.0.9/scarletio/core/traps/future_chaining.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/future_sync_wrapper.py` & `scarletio-1.0.9/scarletio/core/traps/future_sync_wrapper.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/gatherer.py` & `scarletio-1.0.9/scarletio/core/traps/gatherer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/handle_cancellers.py` & `scarletio-1.0.9/scarletio/core/traps/handle_cancellers.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/locks.py` & `scarletio-1.0.9/scarletio/core/traps/locks.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/queues.py` & `scarletio-1.0.9/scarletio/core/traps/queues.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/result_gathering_future.py` & `scarletio-1.0.9/scarletio/core/traps/result_gathering_future.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/task.py` & `scarletio-1.0.9/scarletio/core/traps/task.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/task_suppression.py` & `scarletio-1.0.9/scarletio/core/traps/task_suppression.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/task_thread_switcher.py` & `scarletio-1.0.9/scarletio/core/traps/task_thread_switcher.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/timeouting.py` & `scarletio-1.0.9/scarletio/core/traps/timeouting.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/wait_continously.py` & `scarletio-1.0.9/scarletio/core/traps/wait_continously.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/wait_till_all.py` & `scarletio-1.0.9/scarletio/core/traps/wait_till_all.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/wait_till_exception.py` & `scarletio-1.0.9/scarletio/core/traps/wait_till_exception.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/core/traps/wait_till_first.py` & `scarletio-1.0.9/scarletio/core/traps/wait_till_first.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/__init__.py` & `scarletio-1.0.9/scarletio/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/client_request.py` & `scarletio-1.0.9/scarletio/http_client/client_request.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/client_response.py` & `scarletio-1.0.9/scarletio/http_client/client_response.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/connection.py` & `scarletio-1.0.9/scarletio/http_client/connection.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/connection_key.py` & `scarletio-1.0.9/scarletio/http_client/connection_key.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/connector.py` & `scarletio-1.0.9/scarletio/http_client/connector.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/fingerprint.py` & `scarletio-1.0.9/scarletio/http_client/fingerprint.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/http_client.py` & `scarletio-1.0.9/scarletio/http_client/http_client.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/request_context_managers.py` & `scarletio-1.0.9/scarletio/http_client/request_context_managers.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/http_client/request_info.py` & `scarletio-1.0.9/scarletio/http_client/request_info.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/__init__.py` & `scarletio-1.0.9/scarletio/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .analyzer import *
 from .async_utils import *
 from .base_method import *
 from .code import *
 from .compact import *
+from .dict_iterator_bases import *
 from .dict_update_iterable_iterator import *
 from .docs import *
 from .export_include import *
 from .function_tools import *
 from .hybrid_value_dictionary import *
 from .ignore_case_multi_value_dictionary import *
 from .ignore_case_string import *
@@ -22,22 +23,24 @@
 from .trace import *
 from .type_methodizer import *
 from .type_modulizer import *
 from .weak_core import *
 from .weak_item_dictionary import *
 from .weak_key_dictionary import *
 from .weak_map import *
+from .weak_set import *
 from .weak_value_dictionary import *
 
 __all__ = (
     *analyzer.__all__,
     *async_utils.__all__,
     *base_method.__all__,
     *code.__all__,
     *compact.__all__,
+    *dict_iterator_bases.__all__,
     *dict_update_iterable_iterator.__all__,
     *docs.__all__,
     *export_include.__all__,
     *function_tools.__all__,
     *hybrid_value_dictionary.__all__,
     *ignore_case_multi_value_dictionary.__all__,
     *ignore_case_string.__all__,
@@ -53,9 +56,10 @@
     *trace.__all__,
     *type_methodizer.__all__,
     *type_modulizer.__all__,
     *weak_core.__all__,
     *weak_item_dictionary.__all__,
     *weak_key_dictionary.__all__,
     *weak_map.__all__,
+    *weak_set.__all__,
     *weak_value_dictionary.__all__,
 )
```

### Comparing `scarletio-1.0.8/scarletio/utils/analyzer.py` & `scarletio-1.0.9/scarletio/utils/analyzer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/async_utils.py` & `scarletio-1.0.9/scarletio/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/base_method.py` & `scarletio-1.0.9/scarletio/utils/base_method.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/dict_update_iterable_iterator.py` & `scarletio-1.0.9/scarletio/utils/dict_update_iterable_iterator.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/docs.py` & `scarletio-1.0.9/scarletio/utils/docs.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/export_include.py` & `scarletio-1.0.9/scarletio/utils/export_include.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/function_tools.py` & `scarletio-1.0.9/scarletio/utils/function_tools.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/hybrid_value_dictionary.py` & `scarletio-1.0.9/scarletio/utils/hybrid_value_dictionary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,22 @@
 __all__ = ('HybridValueDictionary', )
 
+from .dict_iterator_bases import DictionaryItemIteratorBase, DictionaryKeyIteratorBase, DictionaryValueIteratorBase
 from .dict_update_iterable_iterator import _dict_update_iterable_iterator
-from .docs import has_docs
+from .docs import copy_docs, has_docs
 from .weak_core import KeyedReferer, add_to_pending_removals, is_weakreferable
 from .weak_value_dictionary import _WeakValueDictionaryCallback
 
 
-@has_docs
-class _HybridValueDictionaryKeyIterator:
-    """
-    Key iterator for ``HybridValueDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``HybridValueDictionary``
-        The parent hybrid value dictionary.
-    """
-    __slots__ = ('_parent',)
+class _HybridValueDictionaryKeyIterator(DictionaryKeyIteratorBase):
+    __slots__ = ()
     
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_HybridValueDictionaryKeyIterator`` bound to the given ``HybridValueDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``HybridValueDictionary``
-            The parent hybrid value dictionary.
-        """
-        self._parent = parent
     
-    @has_docs
+    @copy_docs(DictionaryKeyIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a hybrid value dictionary's keys.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        key : `Any`
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for key, (value_weakreferable, value_or_reference) in dict.items(parent):
                 if value_weakreferable and (value_or_reference() is None):
                     add_to_pending_removals(parent, value_or_reference)
@@ -53,60 +25,25 @@
                 yield key
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
-    @has_docs
+    
+    @copy_docs(DictionaryKeyIteratorBase.__contains__)
     def __contains__(self, contains_key):
-        """Returns whether the respective ``HybridValueDictionary`` contains the given key."""
         return (contains_key in self._parent)
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``HybridValueDictionary``'s length."""
-        return len(self._parent)
 
 
-@has_docs
-class _HybridValueDictionaryValueIterator:
-    """
-    Value iterator for ``HybridValueDictionary``-s.
+class _HybridValueDictionaryValueIterator(DictionaryValueIteratorBase):
+    __slots__ = ()
     
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``HybridValueDictionary``
-        The parent hybrid value dictionary.
-    """
-    __slots__ = ('_parent',)
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_HybridValueDictionaryValueIterator`` bound to the given ``HybridValueDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``HybridValueDictionary``
-            The parent hybrid value dictionary.
-        """
-        self._parent = parent
-    
-    @has_docs
+    @copy_docs(DictionaryValueIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a hybrid value dictionary's values.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        value : `Any`
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for value_weakreferable, value_or_reference in dict.values(parent):
                 if value_weakreferable:
                     value = value_or_reference()
@@ -119,17 +56,17 @@
                 yield value
                 continue
         
         finally:
             parent._iterating -=1
             parent._commit_removals()
     
-    @has_docs
+    
+    @copy_docs(DictionaryValueIteratorBase.__contains__)
     def __contains__(self, contains_value):
-        """Returns whether the respective ``HybridValueDictionary`` contains the given value."""
         parent = self._parent
         for value_weakreferable, value_or_reference in dict.values(parent):
             if value_weakreferable:
                 value = value_or_reference()
                 if value is None:
                     add_to_pending_removals(parent, value_or_reference)
                     continue
@@ -141,56 +78,21 @@
                 break
         else:
             result = False
         
         parent._commit_removals()
         
         return result
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``HybridValueDictionary``'s length."""
-        return len(self._parent)
 
 
-@has_docs
-class _HybridValueDictionaryItemIterator:
-    """
-    Item iterator for ``HybridValueDictionary``-s.
+class _HybridValueDictionaryItemIterator(DictionaryItemIteratorBase):
+    __slots__ = ()
     
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``HybridValueDictionary``
-        The parent hybrid value dictionary.
-    """
-    __slots__ = ('_parent',)
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_HybridValueDictionaryItemIterator`` bound to the given ``HybridValueDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``HybridValueDictionary``
-            The parent hybrid value dictionary.
-        """
-        self._parent = parent
-    
-    @has_docs
+    @copy_docs(DictionaryItemIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a hybrid value dictionary's items.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        item : `tuple` (`Any`, `Any`)
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for key, (value_weakreferable, value_or_reference) in dict.items(parent):
                 if value_weakreferable:
                     value = value_or_reference()
@@ -203,17 +105,17 @@
                 yield key, value
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
-    @has_docs
+    
+    @copy_docs(DictionaryItemIteratorBase.__contains__)
     def __contains__(self, contains_item):
-        """Returns whether the respective ``HybridValueDictionary`` contains the given item."""
         if not isinstance(contains_item, tuple):
             return False
         
         if len(contains_item) != 2:
             return False
         
         parent = self._parent
@@ -233,19 +135,14 @@
                     dict.__delitem__(parent, contains_key)
                 
                 return False
         else:
             value = value_or_reference
         
         return (value == contains_value)
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``HybridValueDictionary``'s length."""
-        return len(self._parent)
 
 
 @has_docs
 class HybridValueDictionary(dict):
     """
     Hybrid value dictionaries store their's values weakly referenced if applicable.
     
@@ -326,15 +223,36 @@
         
         return True
     
     # __delattr__ -> same
     # __delitem__ -> same
     # __dir__ -> same
     # __doc__ -> same
-    # __eq__ -> same
+    
+    def __eq__(self, other):
+        """Returns whether the two dictionaries are the same."""
+        if isinstance(other, type(self)):
+            return dict.__eq__(self, other)
+        
+        if isinstance(other, dict):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            try:
+                other = dict(other)
+            except (TypeError, ValueError):
+                return NotImplemented
+            
+        else:
+            return NotImplemented
+        
+        self_dict = dict(self.items())
+        
+        return self_dict == other
+    
     # __format__ -> same
     # __ge__ -> same
     # __getattribute__ -> same
     
     @has_docs
     def __getitem__(self, key):
         """Gets the value of the hybrid value dictionary which matches the given key."""
@@ -388,18 +306,50 @@
         pending_removals = self._pending_removals
         if (pending_removals is not None):
             length -= len(pending_removals)
         
         return length
     
     # __lt__ -> same
-    # __ne__ -> same
+    
+    
+    def __ne__(self, other):
+        """Returns whether the two dictionaries are different."""
+        if isinstance(other, type(self)):
+            return dict.__ne__(self, other)
+        
+        if isinstance(other, dict):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            try:
+                other = dict(other)
+            except (TypeError, ValueError):
+                return NotImplemented
+        
+        else:
+            return NotImplemented
+        
+        self_dict = dict(self.items())
+        
+        return self_dict != other
+    
     # __new__ -> same
-    # __reduce__ -> we do not care
-    # __reduce_ex__ -> we do not care
+    
+    @has_docs
+    def __reduce__(self):
+        """Reduces the dictionary to a picklable object."""
+        return (type(self), list(self.items()))
+    
+    
+    @has_docs
+    def __reduce_ex__(self, version):
+        """Reduces the dictionary to a picklable object."""
+        return type(self).__reduce__(self)
+    
     
     @has_docs
     def __repr__(self):
         """Returns the representation of the hybrid value dictionary."""
         result = [self.__class__.__name__, '({']
         if len(self):
             limit = self.MAX_REPR_ELEMENT_LIMIT
```

### Comparing `scarletio-1.0.8/scarletio/utils/ignore_case_string.py` & `scarletio-1.0.9/scarletio/utils/ignore_case_string.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/json.py` & `scarletio-1.0.9/scarletio/utils/json.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/keep_type.py` & `scarletio-1.0.9/scarletio/utils/keep_type.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/method_like.py` & `scarletio-1.0.9/scarletio/utils/method_like.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/multi_value_dictionary.py` & `scarletio-1.0.9/scarletio/utils/multi_value_dictionary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,123 +1,80 @@
 __all__ = ('MultiValueDictionary', )
 
-from .docs import has_docs
+from .dict_iterator_bases import DictionaryItemIteratorBase, DictionaryValueIteratorBase
+from .docs import copy_docs, has_docs
 from .removed_descriptor import RemovedDescriptor
-
+from .utils import is_iterable
 
 @has_docs
-class _MultiValueDictionaryItemIterator:
-    """
-    ``MultiValueDictionary`` item iterator.
-    
-    Attributes
-    ----------
-    _parent : ``MultiValueDictionary``
-        The parent MultiValueDictionary.
-    """
-    __slots__ = ('_parent',)
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``MultiValueDictionary`` item iterator.
-        
-        Parameters
-        ----------
-        parent : ``MultiValueDictionary``
-            The parent multi value dictionary.
-        """
-        self._parent = parent
-    
+class _MultiValueDictionaryItemIterator(DictionaryItemIteratorBase):
+    __slots__ = ()
     
-    @has_docs
+    @copy_docs(DictionaryItemIteratorBase.__len__)
     def __len__(self):
-        """Returns the respective ``MultiValueDictionary``'s length."""
-        return len(self._parent)
+        length = 0
+        
+        for values in dict.values(self._parent):
+            length += len(values)
+        
+        return length
     
     
-    @has_docs
+    @copy_docs(DictionaryItemIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over the respective ``MultiValueDictionary``'s items.
-        
-        This method is a generator.
-        
-        Yields
-        -------
-        item : `tuple` (`Any`, `Any`)
-            Items of the respective MultiValueDictionary as `key` - `value` pairs.
-        """
         for key, values in dict.items(self._parent):
             for value in values:
                 yield key, value
     
     
-    @has_docs
+    @copy_docs(DictionaryItemIteratorBase.__contains__)
     def __contains__(self, item):
-        """Returns whether the respective MultiValueDictionary contains the given item."""
+        print(item)
+        if not isinstance(item, tuple):
+            return False
+        
+        if len(item) != 2:
+            return False
+        
         key, value = item
-        parent = self._parent
+        
         try:
-            values = parent[key]
+            values = dict.__getitem__(self._parent, key)
         except KeyError:
             return False
+        
         return value in values
 
 
 @has_docs
-class _MultiValueDictionaryValueIterator:
-    """
-    ``MultiValueDictionary`` value iterator.
-    
-    Attributes
-    ----------
-    _parent : ``MultiValueDictionary``
-        The parent MultiValueDictionary.
-    """
-    __slots__ = ('_parent',)
+class _MultiValueDictionaryValueIterator(DictionaryValueIteratorBase):
+    __slots__ = ()
     
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``MultiValueDictionary`` value iterator.
+    @copy_docs(DictionaryValueIteratorBase.__len__)
+    def __len__(self):
+        length = 0
         
-        Parameters
-        ----------
-        parent : ``MultiValueDictionary``
-            The parent MultiValueDictionary.
-        """
-        self._parent = parent
+        for values in dict.values(self._parent):
+            length += len(values)
+        
+        return length
     
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``MultiValueDictionary``'s length."""
-        return len(self._parent)
     
-    @has_docs
+    @copy_docs(DictionaryValueIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over the respective ``MultiValueDictionary``'s values.
-        
-        This method is a generator.
-        
-        Yields
-        -------
-        value : `Any`
-            Values of the respective MultiValueDictionary.
-        """
         for values in dict.values(self._parent):
             yield from values
     
-    @has_docs
+    
+    @copy_docs(DictionaryValueIteratorBase.__contains__)
     def __contains__(self, value):
-        """Returns whether the respective MultiValueDictionary contains the given value."""
         for values in dict.values(self._parent):
             if value in values:
                 return True
+        
         return False
 
 
 @has_docs
 class MultiValueDictionary(dict):
     """
     Dictionary subclass, which can hold multiple values bound to a single key.
@@ -128,23 +85,21 @@
     def __init__(self, iterable=None):
         """
         Creates a new ``MultiValueDictionary``.
         
         Parameters
         ----------
         iterable : `None`, `iterable`, Optional
-            Iterable to update the created MultiValueDictionary initially.
+            Iterable to update the created dictionary initially.
             
             Can be given as one of the following:
                 - ``MultiValueDictionary``.
                 - `dict`.
                 - `iterable` of `key` - `value` pairs.
         """
-        dict.__init__(self)
-        
         if (iterable is None) or (not iterable):
             return
         
         getitem = dict.__getitem__
         setitem = dict.__setitem__
         
         if isinstance(iterable, MultiValueDictionary):
@@ -158,101 +113,155 @@
         else:
             for key, value in iterable:
                 try:
                     values = getitem(self, key)
                 except KeyError:
                     setitem(self, key, [value])
                 else:
-                    values.append(value)
+                    if value not in values:
+                        values.append(value)
+    
     
     @has_docs
     def __getitem__(self, key):
         """
-        Returns the MultiValueDictionary's `value` for the given `key`. If the `key` has more values, then returns the 0th of
+        Returns the dictionary's `value` for the given `key`. If the `key` has more values, then returns the 0th of
         them.
         """
         return dict.__getitem__(self, key)[0]
     
+    
     @has_docs
     def __setitem__(self, key, value):
-        """Adds the given `key` - `value` pair to the MultiValueDictionary."""
+        """Adds the given `key` - `value` pair to the dictionary."""
         try:
             line = dict.__getitem__(self, key)
         except KeyError:
             dict.__setitem__(self, key, [value])
         else:
             if value not in line:
                 line.append(value)
     
+    
     @has_docs
     def __delitem__(self, key):
         """
-        Removes the `value` for the given `key` from the MultiValueDictionary. If the `key` has more values, then removes only
+        Removes the `value` for the given `key` from the dictionary. If the `key` has more values, then removes only
         the 0th of them.
         """
         my_list = dict.__getitem__(self, key)
         if len(my_list) == 1:
             dict.__delitem__(self, key)
         else:
             del my_list[0]
     
+    
+    @has_docs
+    def __eq__(self, other):
+        """Returns whether the dictionary equals to other."""
+        if isinstance(other, type(self)):
+            return dict.__eq__(self, other)
+        
+        if is_iterable(other):
+            try:
+                other = type(self)(other)
+            except TypeError:
+                return NotImplemented
+            
+            return dict.__eq__(self, other)
+        
+        return NotImplemented
+    
+    
+    @has_docs
+    def __ne__(self, other):
+        """Returns whether the dictionary equals to other."""
+        if isinstance(other, type(self)):
+            return dict.__ne__(self, other)
+        
+        if is_iterable(other):
+            try:
+                other = type(self)(other)
+            except TypeError:
+                return NotImplemented
+            
+            return dict.__ne__(self, other)
+        
+        return NotImplemented
+    
+    
+    @has_docs
+    def __reduce__(self):
+        """Reduces the dictionary to a picklable object."""
+        return (type(self), list(self.items()))
+    
+    
+    @has_docs
+    def __reduce_ex__(self, version):
+        """Reduces the dictionary to a picklable object."""
+        return type(self).__reduce__(self)
+    
+    
     @has_docs
     def extend(self, mapping):
         """
-        Extends the MultiValueDictionary with the given `mapping`'s items.
+        Extends the dictionary with the given `mapping`'s items.
         
         Parameters
         ----------
         mapping : `Any`
             Any mapping type, what has `.items` attribute.
         """
         getitem = dict.__getitem__
         setitem = dict.__setitem__
+        
         for key, value in mapping.items():
             try:
                 values = getitem(self, key)
             except KeyError:
                 setitem(self, key, [value])
             else:
                 if value not in values:
                     values.append(value)
     
+    
     @has_docs
     def get_all(self, key, default=None):
         """
         Returns all the values matching the given `key`.
         
         Parameters
         ----------
         key : `Any`
             The `key` to match.
         default : `Any`, Optional
-            Default value to return if `key` is not present in the MultiValueDictionary. Defaults to `None`.
+            Default value to return if `key` is not present in the dictionary. Defaults to `None`.
         
         Returns
         -------
         values : `default or `list` of `Any`
             The values for the given `key` if present.
         """
         try:
             return dict.__getitem__(self, key).copy()
         except KeyError:
             return default
     
+    
     @has_docs
     def get_one(self, key, default=None):
         """
         Returns the 0th value matching the given `key`.
         
         Parameters
         ----------
         key : `Any`
             The key to match.
         default : `Any`, Optional
-            Default value to return if `key` is not present in the MultiValueDictionary. Defaults to `None`.
+            Default value to return if `key` is not present in the dictionary. Defaults to `None`.
         
         Returns
         -------
         value : `default`, `Any`
             The value for the given key if present.
         """
         try:
@@ -265,22 +274,22 @@
     get = get_one
     
     @has_docs
     def setdefault(self, key, default=None):
         """
         Returns the value for the given `key`.
         
-        If the `key` is not present in the MultiValueDictionary, then set's the given `default` value as it.
+        If the `key` is not present in the dictionary, then set's the given `default` value as it.
         
         Parameters
         ----------
         key : `Any`
             The key to match.
         default : `Any`, Optional
-            Default value to set and return if `key` is not present in the MultiValueDictionary.
+            Default value to set and return if `key` is not present in the dictionary.
         
         Returns
         -------
         value : `default`, `Any`
             The first value for which `key` matched, or `default` if none.
         """
         try:
@@ -289,64 +298,66 @@
             pass
         else:
             return values[0]
         
         dict.__setitem__(self, key, [default])
         return default
     
+    
     @has_docs
     def pop_all(self, key, default=...):
         """
-        Removes all the values from the MultiValueDictionary which the given `key` matched.
+        Removes all the values from the dictionary which the given `key` matched.
         
         Parameters
         ----------
         key : `Any`
             The key to match.
         default : `Any`, Optional
-            Default value to return if `key` is not present in the MultiValueDictionary.
+            Default value to return if `key` is not present in the dictionary.
         
         Returns
         -------
         values : `default`, `list` of `Any`
             The matched values. If `key` is not present, but `default` value is given, then returns that.
         
         Raises
         ------
         KeyError
-            if `key` is not present in the MultiValueDictionary and `default` value is not given either.
+            if `key` is not present in the dictionary and `default` value is not given either.
         """
         try:
             return dict.pop(self, key)
         except KeyError:
             if default is not ...:
                 return default
             raise
     
+    
     @has_docs
     def pop_one(self, key, default=...):
         """
-        Removes the first value from the MultiValueDictionary, which matches the given `key`.
+        Removes the first value from the dictionary, which matches the given `key`.
         
         Parameters
         ----------
         key : `Any`
             The key to match.
         default : `Any`, Optional
-            Default value to return if `key` is not present in the MultiValueDictionary.
+            Default value to return if `key` is not present in the dictionary.
         
         Returns
         -------
         value : `default`, `list` of `Any`
             The 0th matched value. If `key` is not present, but `default` value is given, then returns that.
         
         Raises
         ------
         KeyError
-            if `key` is not present in the MultiValueDictionary and `default` value is not given either.
+            if `key` is not present in the dictionary and `default` value is not given either.
         """
         try:
             values = dict.__getitem__(self, key)
         except KeyError:
             if default is not ...:
                 return default
             raise
@@ -355,61 +366,88 @@
             if not values:
                 dict.__delitem__(self, key)
             
             return value
     
     pop = pop_one
     
-    # inheritable:
+    
+    @has_docs
+    def popitem(self):
+        """
+        Pops an item of the dictionary.
+        
+        Returns
+        -------
+        item : `tuple` (`Any`, `Any`)
+        
+        Raises
+        ------
+        KeyError
+            If the dictionary is empty.
+        """
+        key, values = dict.popitem(self)
+        value = values.pop(0)
+        
+        if values:
+            dict.__setitem__(self, key, values)
+        
+        return key, value
+        
+        raise KeyError('popitem(): dictionary is empty.')
+    
+    
     @has_docs
     def copy(self):
         """
-        Copies the MultiValueDictionary.
+        Copies the dictionary.
         
         Returns
         -------
         new : ``MultiValueDictionary``
-            The new MultiValueDictionary.
         """
         new = dict.__new__(type(self))
         setitem = dict.__setitem__
         for key, values in dict.items(self):
             setitem(new, key, values.copy())
         
         return new
     
+    
     @has_docs
     def items(self):
         """
-        Returns an item iterator for the MultiValueDictionary.
+        Returns an item iterator for the dictionary.
         
         Returns
         -------
         items : ``_MultiValueDictionaryItemIterator``
         """
         return _MultiValueDictionaryItemIterator(self)
     
+    
     @has_docs
     def values(self):
         """
-        Returns a value iterator for the MultiValueDictionary.
+        Returns a value iterator for the dictionary.
         
         Returns
         -------
         items : ``_MultiValueDictionaryValueIterator``
         """
         return _MultiValueDictionaryValueIterator(self)
     
+    
     @has_docs
     def __repr__(self):
-        """Returns the MultiValueDictionary's representation."""
+        """Returns the dictionary's representation."""
         result = [
             self.__class__.__name__,
             '({',
-                ]
+        ]
         
         if self:
             for key, value in self.items():
                 result.append(repr(key))
                 result.append(': ')
                 result.append(repr(value))
                 result.append(', ')
@@ -421,15 +459,15 @@
         return ''.join(result)
     
     __str__ = __repr__
     
     @has_docs
     def kwargs(self):
         """
-        Converts the MultiValueDictionary to `**kwargs`-able dictionary. If a `key` has more values, then always returns the last
+        Converts the dictionary to `**kwargs`-able dictionary. If a `key` has more values, then always returns the last
         value for it.
         
         Returns
         -------
         result : `dict` of (`Any`, `Any`) items
         """
         result = {}
```

### Comparing `scarletio-1.0.8/scarletio/utils/properties.py` & `scarletio-1.0.9/scarletio/utils/properties.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/removed_descriptor.py` & `scarletio-1.0.9/scarletio/utils/removed_descriptor.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/rich_attribute_error.py` & `scarletio-1.0.9/scarletio/utils/rich_attribute_error.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/sorted_list.py` & `scarletio-1.0.9/scarletio/utils/sorted_list.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/trace.py` & `scarletio-1.0.9/scarletio/utils/trace.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/type_methodizer.py` & `scarletio-1.0.9/scarletio/utils/type_methodizer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/type_modulizer.py` & `scarletio-1.0.9/scarletio/utils/type_modulizer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/utils/utils.py` & `scarletio-1.0.9/scarletio/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = (
-    'IS_UNIX', 'any_to_any', 'change_on_switch', 'get_short_executable', 'list_difference', 'relative_index',
-    'un_map_pack', 'where'
+    'IS_UNIX', 'any_to_any', 'change_on_switch', 'get_short_executable', 'is_hashable', 'is_iterable',
+    'list_difference', 'relative_index', 'un_map_pack', 'where'
 )
 
 import sys
 from os import sep as PATH_SEPARATOR
 
 from .docs import has_docs
 
@@ -330,7 +330,50 @@
         return key
     
     @has_docs
     def __getitem__(self, key):
         """Gets the next value of the un-map-packer."""
         return self.next_value
 
+
+@has_docs
+def is_iterable(object_):
+    """
+    Returns whether the object is iterable.
+    
+    Parameters
+    ----------
+    object_ : `Any`
+        The object to check.
+    
+    Returns
+    -------
+    is_iterable : `bool`
+    """
+    return hasattr(type(object_), '__iter__')
+
+
+@has_docs
+def is_hashable(object_):
+    """
+    Returns whether the object is hashable.
+    
+    Parameters
+    ----------
+    object_ : `Any`
+        The object to check.
+    
+    Returns
+    -------
+    is_iterable : `bool`
+    """
+    try:
+        hasher_function = getattr(type(object_), '__hash__')
+    except AttributeError:
+        return False
+    
+    try:
+        hasher_function(object_)
+    except (TypeError, NotImplementedError):
+        return False
+    
+    return True
```

### Comparing `scarletio-1.0.8/scarletio/utils/weak_core.py` & `scarletio-1.0.9/scarletio/utils/weak_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,29 @@
     """
     __slots__ = ()
     if NEEDS_DUMMY_INIT:
         def __init__(self, *args, **kwargs):
             pass
     else:
         __init__ = object.__init__
+    
+    
+    def __repr__(self):
+        repr_parts = ['<', self.__class__.__name__]
+        
+        value = self()
+        if value is None:
+            repr_parts.append(' (dead)')
+        else:
+            repr_parts.append(' value=')
+            repr_parts.append(repr(value))
+        
+        repr_parts.append('>')
+        return ''.join(repr_parts)
+
 
 del WeakrefType
 
 
 @has_docs
 class KeyedReferer(WeakReferer):
     """
```

### Comparing `scarletio-1.0.8/scarletio/utils/weak_item_dictionary.py` & `scarletio-1.0.9/scarletio/utils/weak_item_dictionary.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = ('WeakItemDictionary',)
 
+from .dict_iterator_bases import DictionaryItemIteratorBase, DictionaryValueIteratorBase
 from .dict_update_iterable_iterator import _dict_update_iterable_iterator
-from .docs import has_docs
+from .docs import copy_docs, has_docs
 from .weak_core import KeyedReferer, WeakReferer, add_to_pending_removals
 from .weak_key_dictionary import _WeakKeyDictionaryCallback, _WeakKeyDictionaryKeyIterator
 
 
 @has_docs
 class _WeakItemDictionaryValueCallback:
     """
@@ -55,51 +56,19 @@
         else:
             try:
                 dict.__delitem__(parent, key_reference)
             except KeyError:
                 pass
 
 
-@has_docs
-class _WeakItemDictionaryValueIterator:
-    """
-    Value iterator for ``WeakValueDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakValueDictionary``
-        The parent weak value dictionary.
-    """
-    __slots__ = ('_parent',)
+class _WeakItemDictionaryValueIterator(DictionaryValueIteratorBase):
+    __slots__ = ()
     
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakValueDictionaryValueIterator`` bound to the given ``WeakValueDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``WeakValueDictionary``
-            The parent weak value dictionary.
-        """
-        self._parent = parent
-    
-    
-    @has_docs
+    @copy_docs(DictionaryValueIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a weak value dictionary's values.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        value : `Any`
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for value_reference in dict.values(parent):
                 value = value_reference()
                 if (value is None):
@@ -110,17 +79,16 @@
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
     
-    @has_docs
+    @copy_docs(DictionaryValueIteratorBase.__contains__)
     def __contains__(self, contains_value):
-        """Returns whether the respective ``WeakValueDictionary`` contains the given value."""
         parent = self._parent
         for value_reference in dict.values(parent):
             value = value_reference()
             if (value is None):
                 add_to_pending_removals(parent, value_reference.key)
                 continue
             
@@ -132,59 +100,23 @@
             result = False
         
         parent._commit_removals()
         
         return result
     
     
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakValueDictionary``'s length."""
-        return len(self._parent)
-
-
 
-@has_docs
-class _WeakItemDictionaryItemIterator:
-    """
-    Item iterator for ``WeakItemDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakItemDictionary``
-        The parent weak item dictionary.
-    """
-    __slots__ = ('_parent',)
+class _WeakItemDictionaryItemIterator(DictionaryItemIteratorBase):
+    __slots__ = ()
     
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakItemDictionaryItemIterator`` bound to the given ``WeakItemDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``WeakItemDictionary``
-            The parent weak item dictionary.
-        """
-        self._parent = parent
-    
-    
-    @has_docs
+    @copy_docs(DictionaryItemIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a weak item dictionary's items.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        item : `tuple` (`Any`, `Any`)
-        """
         parent = self._parent
-        parent._iterating += 1
+        iterating = parent._iterating
+        parent._iterating = iterating + 1
         
         try:
             for key_reference, value_reference in dict.items(parent):
                 key = key_reference()
                 if (key is None):
                     add_to_pending_removals(parent, key_reference)
                     continue
@@ -198,17 +130,16 @@
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
     
-    @has_docs
+    @copy_docs(DictionaryItemIteratorBase.__contains__)
     def __contains__(self, contains_item):
-        """Returns whether the respective ``WeakItemDictionary`` contains the given item."""
         if not isinstance(contains_item, tuple):
             return False
         
         if len(contains_item) != 2:
             return False
         
         parent = self._parent
@@ -230,21 +161,14 @@
                 add_to_pending_removals(parent, value_reference.key)
             else:
                 dict.__delitem__(parent, value_reference.key)
             
             return False
         
         return (value == contains_value)
-    
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakItemDictionary``'s length."""
-        return len(self._parent)
-
 
 
 @has_docs
 class WeakItemDictionary(dict):
     """
     weak item dictionary, which stores it's values weakly referenced.
     
@@ -327,36 +251,57 @@
         except TypeError:
             raise KeyError(key) from None
         
         dict.__delitem__(self, key)
     
     # __dir__ -> same
     # __doc__ -> same
-    # __eq__ -> same
+    
+    def __eq__(self, other):
+        """Returns whether the two dictionaries are the same."""
+        if isinstance(other, type(self)):
+            return dict.__eq__(self, other)
+        
+        if isinstance(other, dict):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            try:
+                other = dict(other)
+            except (ValueError, TypeError):
+                return NotImplemented
+        
+        else:
+            return NotImplemented
+        
+        self_dict = dict(self.items())
+        
+        return self_dict == other
+    
     # __format__ -> same
     # __ge__ -> same
     # __getattribute__ -> same
     
     @has_docs
     def __getitem__(self, key):
         """Gets the value of the weak item dictionary which matches the given key."""
         try:
-            key = WeakReferer(key)
+            key_reference = WeakReferer(key)
         except TypeError:
             raise KeyError(key) from None
         
-        value_reference = dict.__getitem__(self, key)
+        value_reference = dict.__getitem__(self, key_reference)
         value = value_reference()
         if (value is not None):
             return value
         
         if self._iterating:
             add_to_pending_removals(self, value_reference.key)
         else:
-            dict.__delitem__(self, key)
+            dict.__delitem__(self, value_reference.key)
         
         raise KeyError(key)
     
     # __gt__ -> same
     # __hash__ -> same
     
     @has_docs
@@ -392,18 +337,49 @@
         pending_removals = self._pending_removals
         if (pending_removals is not None):
             length -= len(pending_removals)
         
         return length
     
     # __lt__ -> same
-    # __ne__ -> same
+    
+    def __ne__(self, other):
+        """Returns whether the two dictionaries are different."""
+        if isinstance(other, type(self)):
+            return dict.__ne__(self, other)
+        
+        if isinstance(other, dict):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            try:
+                other = dict(other)
+            except (ValueError, TypeError):
+                return NotImplemented
+        
+        else:
+            return NotImplemented
+        
+        self_dict = dict(self.items())
+        
+        return self_dict != other
+    
     # __new__ -> same
-    # __reduce__ -> we do not care
-    # __reduce_ex__ -> we do not care
+    
+    @has_docs
+    def __reduce__(self):
+        """Reduces the dictionary to a picklable object."""
+        return (type(self), list(self.items()))
+    
+    
+    @has_docs
+    def __reduce_ex__(self, version):
+        """Reduces the dictionary to a picklable object."""
+        return type(self).__reduce__(self)
+    
     
     @has_docs
     def __repr__(self):
         """Returns the representation of the weak item dictionary."""
         result = [self.__class__.__name__, '({']
         
         if len(self):
@@ -481,14 +457,15 @@
         """
         new = dict.__new__(type(self))
         new._pending_removals = None
         key_callback = _WeakKeyDictionaryCallback(new)
         new._key_callback = key_callback
         value_callback = _WeakItemDictionaryValueCallback(new)
         new._value_callback = value_callback
+        new._iterating = 0
         
         for key_reference, value_reference in dict.items(self):
             key = key_reference()
             if key is None:
                 add_to_pending_removals(self, key_reference)
                 continue
```

### Comparing `scarletio-1.0.8/scarletio/utils/weak_key_dictionary.py` & `scarletio-1.0.9/scarletio/utils/weak_key_dictionary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = ('WeakKeyDictionary',)
 
+from .dict_iterator_bases import DictionaryItemIteratorBase, DictionaryKeyIteratorBase, DictionaryValueIteratorBase
 from .dict_update_iterable_iterator import _dict_update_iterable_iterator
-from .docs import has_docs
+from .docs import copy_docs, has_docs
 from .weak_core import WeakReferer, add_to_pending_removals
 
 
 @has_docs
 class _WeakKeyDictionaryCallback:
     """
     Callback used by ``WeakKeyDictionary``-s.
@@ -52,49 +53,19 @@
         else:
             try:
                 dict.__delitem__(parent, reference)
             except KeyError:
                 pass
 
 
-@has_docs
-class _WeakKeyDictionaryKeyIterator:
-    """
-    Key iterator for ``WeakKeyDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakKeyDictionary``
-        The parent weak key dictionary.
-    """
-    __slots__ = ('_parent',)
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakKeyDictionaryKeyIterator`` bound to the given ``WeakKeyDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``WeakKeyDictionary``
-            The parent weak key dictionary.
-        """
-        self._parent = parent
+class _WeakKeyDictionaryKeyIterator(DictionaryKeyIteratorBase):
+    __slots__ = ()
     
-    @has_docs
+    @copy_docs(DictionaryKeyIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a weak key dictionary's keys.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        key : `Any`
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for key_reference in dict.keys(parent):
                 key = key_reference()
                 if (key is None):
@@ -104,60 +75,25 @@
                 yield key
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
-    @has_docs
+    
+    @copy_docs(DictionaryKeyIteratorBase.__contains__)
     def __contains__(self, contains_key):
-        """Returns whether the respective ``WeakKeyDictionary`` contains the given key."""
         return (contains_key in self._parent)
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakKeyDictionary``'s length."""
-        return len(self._parent)
 
 
-@has_docs
-class _WeakKeyDictionaryValueIterator:
-    """
-    Value iterator for ``WeakKeyDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakKeyDictionary``
-        The parent weak key dictionary.
-    """
-    __slots__ = ('_parent',)
+class _WeakKeyDictionaryValueIterator(DictionaryValueIteratorBase):
+    __slots__ = ()
     
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakKeyDictionaryValueIterator`` bound to the given ``WeakKeyDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``WeakKeyDictionary``
-            The parent weak key dictionary.
-        """
-        self._parent = parent
-    
-    @has_docs
+    @copy_docs(DictionaryValueIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a weak key dictionary's values.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        value : `Any`
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for key_reference, value in dict.items(parent):
                 if (key_reference() is None):
                     add_to_pending_removals(parent, key_reference)
@@ -166,17 +102,17 @@
                 yield value
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
-    @has_docs
+    
+    @copy_docs(DictionaryValueIteratorBase.__contains__)
     def __contains__(self, contains_value):
-        """Returns whether the respective ``WeakKeyDictionary`` contains the given value."""
         parent = self._parent
         
         for key_reference, value in dict.items(parent):
             if (key_reference() is None):
                 add_to_pending_removals(parent, key_reference)
                 continue
             
@@ -187,57 +123,20 @@
         else:
             result = False
         
         parent._commit_removals()
         
         return result
     
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakKeyDictionary``'s length."""
-        return len(self._parent)
 
-
-@has_docs
-class _WeakKeyDictionaryItemIterator:
-    """
-    Item iterator for ``WeakKeyDictionary``-s.
+class _WeakKeyDictionaryItemIterator(DictionaryItemIteratorBase):
+    __slots__ = ()
     
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakKeyDictionary``
-        The parent weak key dictionary.
-    """
-    __slots__ = ('_parent',)
-    
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakKeyDictionaryItemIterator`` bound to the given ``WeakKeyDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``WeakKeyDictionary``
-            The parent weak key dictionary.
-        """
-        self._parent = parent
-    
-    
-    @has_docs
+    @copy_docs(DictionaryItemIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a weak key dictionary's items.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        item : `tuple` (`Any`, `Any`)
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for key_reference, value in dict.items(parent):
                 key = key_reference()
                 if (key is None):
@@ -248,17 +147,16 @@
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
     
-    @has_docs
+    @copy_docs(DictionaryItemIteratorBase.__contains__)
     def __contains__(self, contains_item):
-        """Returns whether the respective ``WeakKeyDictionary`` contains the given item."""
         if not isinstance(contains_item, tuple):
             return False
         
         if len(contains_item) != 2:
             return False
         
         contains_key, contains_value = contains_item
@@ -269,20 +167,14 @@
             return False
         
         value = dict.get(self._parent, contains_key_reference)
         if value is None:
             return False
         
         return (value == contains_value)
-    
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakKeyDictionary``'s length."""
-        return len(self._parent)
 
 
 @has_docs
 class WeakKeyDictionary(dict):
     """
     Weak key dictionary, which stores it's keys weakly referenced.
     
@@ -345,15 +237,39 @@
     @has_docs
     def __delitem__(self, key):
         """Deletes the value of the weak key dictionary which matches the given key."""
         dict.__delitem__(self, WeakReferer(key))
     
     # __dir__ -> same
     # __doc__ -> same
-    # __eq__ -> same
+    
+    
+    @has_docs
+    def __eq__(self, other):
+        """Returns whether the two dictionaries are the same."""
+        if isinstance(other, type(self)):
+            return dict.__eq__(self, other)
+        
+        if isinstance(other, dict):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            try:
+                other = dict(other)
+            except (TypeError, ValueError):
+                return NotImplemented
+            
+        else:
+            return NotImplemented
+        
+        self_dict = dict(self.items())
+        
+        return self_dict == other
+    
+    
     # __format__ -> same
     # __ge__ -> same
     # __getattribute__ -> same
     
     @has_docs
     def __getitem__(self, key):
         """Gets the value of the weak key dictionary which matches the given key."""
@@ -394,18 +310,49 @@
         pending_removals = self._pending_removals
         if (pending_removals is not None):
             length -= len(pending_removals)
         
         return length
     
     # __lt__ -> same
-    # __ne__ -> same
+    
+    def __ne__(self, other):
+        """Returns whether the two dictionaries are different."""
+        if isinstance(other, type(self)):
+            return dict.__ne__(self, other)
+        
+        if isinstance(other, dict):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            try:
+                other = dict(other)
+            except (TypeError, ValueError):
+                return NotImplemented
+            
+        else:
+            return NotImplemented
+        
+        self_dict = dict(self.items())
+        
+        return self_dict != other
+    
     # __new__ -> same
-    # __reduce__ -> we do not care
-    # __reduce_ex__ -> we do not care
+    
+    @has_docs
+    def __reduce__(self):
+        """Reduces the dictionary to a picklable object."""
+        return (type(self), list(self.items()))
+    
+    
+    @has_docs
+    def __reduce_ex__(self, version):
+        """Reduces the dictionary to a picklable object."""
+        return type(self).__reduce__(self)
+    
     
     @has_docs
     def __repr__(self):
         """Returns the representation of the weak key dictionary."""
         result = [self.__class__.__name__, '({']
         
         if len(self):
@@ -461,27 +408,29 @@
     def clear(self):
         """
         Clears the weak key dictionary.
         """
         dict.clear(self)
         self._pending_removals = None
     
+    
     @has_docs
     def copy(self):
         """
         Copies the weak key dictionary.
         
         Returns
         -------
         new : ``WeakKeyDictionary``
         """
         new = dict.__new__(type(self))
         new._pending_removals = None
         callback = _WeakKeyDictionaryCallback(new)
         new._callback = callback
+        new._iterating = 0
         
         for key_reference, value in dict.items(self):
             key = key_reference()
             if key is None:
                 add_to_pending_removals(self, key_reference)
                 continue
             
@@ -507,36 +456,39 @@
         Returns
         -------
         value : `Any`, `default`
             The key's matched value. If no value was matched returns the `default` value.
         """
         return dict.get(self, WeakReferer(key), default)
     
+    
     @has_docs
     def items(self):
         """
         Returns item iterator for the weak key dictionary.
         
         Returns
         -------
         item_iterator : ``_WeakKeyDictionaryItemIterator``
         """
         return _WeakKeyDictionaryItemIterator(self)
     
+    
     @has_docs
     def keys(self):
         """
         Returns key iterator for the weak key dictionary.
         
         Returns
         -------
         key_iterator : ``_WeakKeyDictionaryKeyIterator``
         """
         return _WeakKeyDictionaryKeyIterator(self)
     
+    
     @has_docs
     def pop(self, key, default=...):
         """
         Pops the value of the weak key dictionary which matches the given key.
         
         Parameters
         ----------
```

### Comparing `scarletio-1.0.8/scarletio/utils/weak_map.py` & `scarletio-1.0.9/scarletio/utils/weak_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,77 +52,14 @@
             try:
                 dict.__delitem__(parent, reference)
             except KeyError:
                 pass
 
 
 @has_docs
-class _WeakMapIterator:
-    """
-    Iterator for ``WeakKeyDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakMap``
-        The parent weak map.
-    """
-    __slots__ = ('_parent', )
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakMapIterator`` bound to the given ``WeakMap``.
-        
-        Parameters
-        ----------
-        parent : ``WeakMap``
-            The parent weak map.
-        """
-        self._parent = parent
-    
-    @has_docs
-    def __iter__(self):
-        """
-        Iterates over a weak map.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        key : `Any`
-        """
-        parent = self._parent
-        parent._iterating += 1
-        
-        try:
-            for reference in dict.__iter__(parent):
-                key = reference()
-                if (key is None):
-                    add_to_pending_removals(parent, reference)
-                    continue
-                
-                yield key
-                continue
-        
-        finally:
-            parent._iterating -= 1
-            parent._commit_removals()
-    
-    @has_docs
-    def __contains__(self, key):
-        """Returns whether the respective ``WeakMap`` contains the given key."""
-        return (key in self._parent)
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakMap``'s length."""
-        return len(self._parent)
-
-
-@has_docs
 class WeakMap(dict):
     """
     Weak map is a mix of weak dictionaries and weak sets. Can be used to retrieve an already existing weakreferenced
     value from itself.
     
     Attributes
     ----------
@@ -187,33 +124,61 @@
             reference = WeakReferer(key)
         except TypeError:
             raise KeyError(key) from None
         
         try:
             dict.__delitem__(self, reference)
         except KeyError as err:
-            err.args=(key,)
-            raise
+            raise KeyError(key) from None
     
     # __dir__ -> same
     # __doc__ -> same
-    # __eq__ > same
+    
+    def __eq__(self, other):
+        """returns whether the two weak maps are equal."""
+        if isinstance(other, type(self)):
+            return dict.__eq__(self, other)
+        
+        if isinstance(other, set):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            other = set(other)
+        
+        else:
+            return NotImplemented
+        
+        self_set = set(iter(self))
+        
+        return self_set == other
+    
     # __format__ -> same
     # __ge__ -> same
     # __getattribute__ -> same
     
     @has_docs
     def __getitem__(self, key):
         """Gets the already existing key from the weak map, which matches the given one."""
         try:
             reference = WeakReferer(key)
         except TypeError:
             raise KeyError(key) from None
         
-        return dict.__getitem__(self, reference)
+        reference = dict.__getitem__(self, reference)
+        key = reference()
+        if (key is None):
+            if self._iterating:
+                add_to_pending_removals(self, reference)
+            else:
+                dict.__delitem__(self, reference)
+            
+            raise KeyError(key)
+        
+        return key
+    
     
     # __gt__ -> same
     # __hash__ -> same
     
     @has_docs
     def __init__(self, iterable=None):
         """
@@ -230,34 +195,80 @@
         if (iterable is not None):
             self.update(iterable)
     
     # __init_subclass__ -> same
     
     @has_docs
     def __iter__(self):
-        """Returns a ``_WeakMapIterator`` iterating over the weak map's keys."""
-        return iter(_WeakMapIterator(self))
+        """
+        Iterates over the weak map's elements.
+        
+        This method is an iterable generator,
+        """
+        self._iterating += 1
+        
+        try:
+            for reference in dict.__iter__(self):
+                key = reference()
+                if (key is None):
+                    add_to_pending_removals(self, reference)
+                    continue
+                
+                yield key
+                continue
+        
+        finally:
+            self._iterating -= 1
+            self._commit_removals()
     
     # __le__ -> same
     
     @has_docs
     def __len__(self):
         """Returns the length of the weak map."""
         length = dict.__len__(self)
         pending_removals = self._pending_removals
         if (pending_removals is not None):
             length -= len(pending_removals)
         
         return length
     
     # __lt__ -> same
-    # __ne__ -> same
+    
+    def __ne__(self, other):
+        """returns whether the two weak maps are equal."""
+        if isinstance(other, type(self)):
+            return dict.__ne__(self, other)
+        
+        if isinstance(other, set):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            other = set(other)
+        
+        else:
+            return NotImplemented
+        
+        self_set = set(iter(self))
+        
+        return self_set != other
+    
     # __new__ -> same
-    # __reduce__ -> we do not care
-    # __reduce_ex__ -> we do not care
+    
+    @has_docs
+    def __reduce__(self):
+        """Reduces the map to a picklable object."""
+        return (type(self), list(self))
+    
+    
+    @has_docs
+    def __reduce_ex__(self, version):
+        """Reduces the map to a picklable object."""
+        return type(self).__reduce__(self)
+    
     
     @has_docs
     def __repr__(self):
         """Returns the weak map's representation."""
         result = [self.__class__.__name__, '({']
         if len(self):
             limit = self.MAX_REPR_ELEMENT_LIMIT
@@ -305,25 +316,26 @@
     def clear(self):
         """
         Clear's the weak map.
         """
         dict.clear(self)
         self._pending_removals = None
     
+    
     @has_docs
     def copy(self):
         """
         Copies the weak map.
         
         Returns
         -------
         new : ``WeakMap``
         """
         new = dict.__new__(type(self))
-        new._iterating = False
+        new._iterating = 0
         new._pending_removals = None
         new._callback = callback = _WeakMapCallback(new)
         
         for reference in dict.__iter__(self):
             key = reference()
             if (key is None):
                 add_to_pending_removals(self, reference)
@@ -333,14 +345,15 @@
             dict.__setitem__(new, reference, reference)
             continue
         
         self._commit_removals()
         
         return new
     
+    
     @has_docs
     def get(self, key, default=None):
         """
         Gets the key of the weak map, which matches the given one.
         
         Parameters
         ----------
@@ -370,17 +383,19 @@
         if self._iterating:
             add_to_pending_removals(self, real_reference)
         else:
             dict.__delitem__(self, real_reference)
         
         return default
     
+    
     items = RemovedDescriptor()
     keys = RemovedDescriptor()
     
+    
     @has_docs
     def pop(self, key, default=...):
         """
         Pops a key from the weak map which matches the given one.
         
         Parameters
         ----------
@@ -416,19 +431,48 @@
                     dict.__delitem__(self, real_reference)
         
         if default is ...:
             raise KeyError(key)
         
         return default
     
+    
     popitem = RemovedDescriptor()
     setdefault = RemovedDescriptor()
-    update = RemovedDescriptor()
+    
+    
+    @has_docs
+    def update(self, iterable):
+        """
+        Updates the map with the given iterable.
+        
+        Parameters
+        ----------
+        iterable : `iterable`
+            The iterable to update the map with.
+        
+        Raises
+        ------
+        TypeError
+            If the given value is not `iterable`, or any of it's elements is not weakreferable.
+        """
+        if hasattr(type(iterable), '__iter__'):
+            # Make sure, we have unique elements, so convert other to set
+            for element in iterable:
+                self.set(element)
+        
+        else:
+            raise TypeError(
+                f'Parameter `iterable` must be an iterable, got {iterable.__class__.__name__}; {iterable!r}.'
+            )
+    
+    
     values = RemovedDescriptor()
     
+    
     @has_docs
     def set(self, key):
         """
         Sets a key to the ``WeakMap`` and then returns it. If they given key is already present in the ``WeakMap``,
         returns that instead.
         
         Parameters
@@ -436,14 +480,19 @@
         key : `Any`
             A key to match.
         
         Returns
         -------
         real_key : `Any`
             The matched key, or the given one.
+        
+        Raises
+        ------
+        TypeError
+            If `key` not supports weakreferencing.
         """
         reference = WeakReferer(key, self._callback)
         real_reference = dict.get(self, reference, None)
         if (real_reference is not None):
             real_key = real_reference()
             if (real_key is not None):
                 return real_key
```

### Comparing `scarletio-1.0.8/scarletio/utils/weak_value_dictionary.py` & `scarletio-1.0.9/scarletio/utils/weak_value_dictionary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = ('WeakValueDictionary', )
 
+from .dict_iterator_bases import DictionaryItemIteratorBase, DictionaryKeyIteratorBase, DictionaryValueIteratorBase
 from .dict_update_iterable_iterator import _dict_update_iterable_iterator
-from .docs import has_docs
+from .docs import copy_docs, has_docs
 from .weak_core import KeyedReferer, WeakReferer, add_to_pending_removals
 
 
 @has_docs
 class _WeakValueDictionaryCallback:
     """
     Callback used by ``WeakValueDictionary``-s and by ``HybridValueDictionary``-s.
@@ -52,51 +53,19 @@
         else:
             try:
                 dict.__delitem__(parent, reference.key)
             except KeyError:
                 pass
 
 
-@has_docs
-class _WeakValueDictionaryKeyIterator:
-    """
-    Key iterator for ``WeakValueDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakValueDictionary``
-        The parent weak value dictionary.
-    """
-    __slots__ = ('_parent',)
-    
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakValueDictionaryKeyIterator`` bound to the given ``WeakValueDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``WeakValueDictionary``
-            The parent weak value dictionary.
-        """
-        self._parent = parent
-    
+class _WeakValueDictionaryKeyIterator(DictionaryKeyIteratorBase):
+    __slots__ = ()
     
-    @has_docs
+    @copy_docs(DictionaryKeyIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a weak value dictionary's keys.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        key : `Any`
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for key, value_reference in dict.items(parent):
                 if (value_reference() is None):
                     add_to_pending_removals(parent, value_reference)
@@ -106,62 +75,24 @@
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
     
-    @has_docs
+    @copy_docs(DictionaryKeyIteratorBase.__contains__)
     def __contains__(self, key):
-        """Returns whether the respective ``WeakValueDictionary`` contains the given key."""
         return (key in self._parent)
-    
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakValueDictionary``'s length."""
-        return len(self._parent)
 
 
-@has_docs
-class _WeakValueDictionaryValueIterator:
-    """
-    Value iterator for ``WeakValueDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakValueDictionary``
-        The parent weak value dictionary.
-    """
-    __slots__ = ('_parent',)
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakValueDictionaryValueIterator`` bound to the given ``WeakValueDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``WeakValueDictionary``
-            The parent weak value dictionary.
-        """
-        self._parent = parent
+class _WeakValueDictionaryValueIterator(DictionaryValueIteratorBase):
+    __slots__ = ()
     
-    
-    @has_docs
+    @copy_docs(DictionaryValueIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a weak value dictionary's values.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        value : `Any`
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for value_reference in dict.values(parent):
                 value = value_reference()
                 if (value is None):
@@ -172,17 +103,16 @@
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
     
-    @has_docs
+    @copy_docs(DictionaryValueIteratorBase.__contains__)
     def __contains__(self, contains_value):
-        """Returns whether the respective ``WeakValueDictionary`` contains the given value."""
         parent = self._parent
         for value_reference in dict.values(parent):
             value = value_reference()
             if (value is None):
                 add_to_pending_removals(parent, value_reference)
                 continue
             
@@ -192,57 +122,22 @@
         
         else:
             result = False
         
         parent._commit_removals()
         
         return result
-    
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakValueDictionary``'s length."""
-        return len(self._parent)
 
 
 @has_docs
-class _WeakValueDictionaryItemIterator:
-    """
-    Item iterator for ``WeakValueDictionary``-s.
-    
-    Attributes
-    ----------
-    _parent : ``WeakReferer`` to ``WeakValueDictionary``
-        The parent weak value dictionary.
-    """
-    __slots__ = ('_parent',)
-    
-    @has_docs
-    def __init__(self, parent):
-        """
-        Creates a new ``_WeakValueDictionaryItemIterator`` bound to the given ``WeakValueDictionary``.
-        
-        Parameters
-        ----------
-        parent : ``WeakValueDictionary``
-            The parent weak value dictionary.
-        """
-        self._parent = parent
-    
-    @has_docs
+class _WeakValueDictionaryItemIterator(DictionaryItemIteratorBase):
+    __slots__ = ()
+
+    @copy_docs(DictionaryItemIteratorBase.__iter__)
     def __iter__(self):
-        """
-        Iterates over a weak value dictionary's items.
-        
-        This method is a generator.
-        
-        Yields
-        ------
-        item : `tuple` (`Any`, `Any`)
-        """
         parent = self._parent
         parent._iterating += 1
         
         try:
             for key, value_reference in dict.items(parent):
                 value = value_reference()
                 if (value is None):
@@ -252,17 +147,17 @@
                 yield key, value
                 continue
         
         finally:
             parent._iterating -= 1
             parent._commit_removals()
     
-    @has_docs
+    
+    @copy_docs(DictionaryItemIteratorBase.__contains__)
     def __contains__(self, contains_item):
-        """Returns whether the respective ``WeakValueDictionary`` contains the given item."""
         if not isinstance(contains_item, tuple):
             return False
         
         if len(contains_item) != 2:
             return False
         
         parent = self._parent
@@ -279,19 +174,14 @@
                 add_to_pending_removals(parent, value_reference)
             else:
                 dict.__delitem__(parent, contains_key)
             
             return False
         
         return (value == contains_value)
-    
-    @has_docs
-    def __len__(self):
-        """Returns the respective ``WeakValueDictionary``'s length."""
-        return len(self._parent)
 
 
 @has_docs
 class WeakValueDictionary(dict):
     """
     Weak value dictionary, which stores it's values weakly referenced.
     
@@ -366,15 +256,36 @@
         
         return False
     
     # __delattr__ -> same
     # __delitem__ -> same
     # __dir__ -> same
     # __doc__ -> same
-    # __eq__ -> same
+    
+    def __eq__(self, other):
+        """Returns whether the two dictionaries are the same."""
+        if isinstance(other, type(self)):
+            return dict.__eq__(self, other)
+        
+        if isinstance(other, dict):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            try:
+                other = dict(other)
+            except TypeError:
+                return NotImplemented
+        
+        else:
+            return NotImplemented
+        
+        self_dict = dict(self.items())
+        
+        return self_dict == other
+    
     # __format__ -> same
     # __ge__ -> same
     # __getattribute__ -> same
     
     @has_docs
     def __getitem__(self, key):
         """Gets the value of the weak value dictionary which matches the given key."""
@@ -425,18 +336,49 @@
         pending_removals = self._pending_removals
         if (pending_removals is not None):
             length -= len(pending_removals)
         
         return length
     
     # __lt__ -> same
-    # __ne__ -> same
+    
+    def __ne__(self, other):
+        """Returns whether the two dictionaries are different."""
+        if isinstance(other, type(self)):
+            return dict.__ne__(self, other)
+        
+        if isinstance(other, dict):
+            pass
+        
+        elif hasattr(type(other), '__iter__'):
+            try:
+                other = dict(other)
+            except TypeError:
+                return NotImplemented
+        
+        else:
+            return NotImplemented
+        
+        self_dict = dict(self.items())
+        
+        return self_dict != other
+    
     # __new__ -> same
-    # __reduce__ -> we do not care
-    # __reduce_ex__ -> we do not care
+    
+    @has_docs
+    def __reduce__(self):
+        """Reduces the dictionary to a picklable object."""
+        return (type(self), list(self.items()))
+    
+    
+    @has_docs
+    def __reduce_ex__(self, version):
+        """Reduces the dictionary to a picklable object."""
+        return type(self).__reduce__(self)
+    
     
     @has_docs
     def __repr__(self):
         """Returns the representation of the weak value dictionary."""
         result = [self.__class__.__name__, '({']
         
         if len(self):
@@ -491,41 +433,44 @@
     def clear(self):
         """
         Clears the weak value dictionary.
         """
         dict.clear(self)
         self._pending_removals = None
     
+    
     @has_docs
     def copy(self):
         """
         Copies the weak value dictionary.
         
         Returns
         -------
         new : ``WeakValueDictionary``
         """
         new = dict.__new__(type(self))
         new._pending_removals = None
         callback = _WeakValueDictionaryCallback(new)
         new._callback = callback
+        new._iterating = 0
         
         for key, value_reference in dict.items(self):
             value = value_reference()
             if value is None:
                 add_to_pending_removals(self, value_reference)
                 continue
             
             dict.__setitem__(new, key, KeyedReferer(value, callback, key))
             continue
         
         self._commit_removals()
         
         return new
     
+    
     @has_docs
     def get(self, key, default=None):
         """
         Gets the value of the weak value dictionary which matches the given key.
         
         Parameters
         ----------
@@ -550,36 +495,39 @@
         if self._iterating:
             add_to_pending_removals(self, value_reference)
         else:
             dict.__delitem__(self, key)
         
         return default
     
+    
     @has_docs
     def items(self):
         """
         Returns item iterator for the weak value dictionary.
         
         Returns
         -------
         item_iterator : ``_WeakValueDictionaryItemIterator``
         """
         return _WeakValueDictionaryItemIterator(self)
     
+    
     @has_docs
     def keys(self):
         """
         Returns key iterator for the weak value dictionary.
         
         Returns
         -------
         key_iterator : ``_WeakValueDictionaryKeyIterator``
         """
         return _WeakValueDictionaryKeyIterator(self)
     
+    
     @has_docs
     def pop(self, key, default=...):
         """
         Pops the value of the weak value dictionary which matches the given key.
         
         Parameters
         ----------
@@ -605,27 +553,28 @@
                 return value
         
         if default is ...:
             raise KeyError(key)
         
         return default
     
+    
     @has_docs
     def popitem(self):
         """
-        Pops an item of the weak value dictionary.
+        Pops an item of the dictionary.
         
         Returns
         -------
         item : `tuple` (`Any`, `Any`)
         
         Raises
         ------
         KeyError
-            If the weak value dictionary is empty.
+            If the dictionary is empty.
         """
         while dict.__len__(self):
             key, value_reference = dict.popitem(self)
             value = value_reference()
             if (value is not None):
                 return key, value
```

### Comparing `scarletio-1.0.8/scarletio/web_common/__init__.py` & `scarletio-1.0.9/scarletio/web_common/__init__.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/compressors.py` & `scarletio-1.0.9/scarletio/web_common/compressors.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/cookiejar.py` & `scarletio-1.0.9/scarletio/web_common/cookiejar.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/exceptions.py` & `scarletio-1.0.9/scarletio/web_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/formdata.py` & `scarletio-1.0.9/scarletio/web_common/formdata.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/header_building_and_parsing.py` & `scarletio-1.0.9/scarletio/web_common/header_building_and_parsing.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/headers.py` & `scarletio-1.0.9/scarletio/web_common/headers.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/helpers.py` & `scarletio-1.0.9/scarletio/web_common/helpers.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/http_message.py` & `scarletio-1.0.9/scarletio/web_common/http_message.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/http_protocol.py` & `scarletio-1.0.9/scarletio/web_common/http_protocol.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/http_stream_writer.py` & `scarletio-1.0.9/scarletio/web_common/http_stream_writer.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/mime_type.py` & `scarletio-1.0.9/scarletio/web_common/mime_type.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/multipart.py` & `scarletio-1.0.9/scarletio/web_common/multipart.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/quoting.py` & `scarletio-1.0.9/scarletio/web_common/quoting.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/url.py` & `scarletio-1.0.9/scarletio/web_common/url.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/web_common/websocket_frame.py` & `scarletio-1.0.9/scarletio/web_common/websocket_frame.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/websocket/websocket_client.py` & `scarletio-1.0.9/scarletio/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/websocket/websocket_common_protocol.py` & `scarletio-1.0.9/scarletio/websocket/websocket_common_protocol.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/websocket/websocket_server.py` & `scarletio-1.0.9/scarletio/websocket/websocket_server.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio/websocket/websocket_server_protocol.py` & `scarletio-1.0.9/scarletio/websocket/websocket_server_protocol.py`

 * *Files identical despite different names*

### Comparing `scarletio-1.0.8/scarletio.egg-info/SOURCES.txt` & `scarletio-1.0.9/scarletio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 scarletio/http_client/request_info.py
 scarletio/utils/__init__.py
 scarletio/utils/analyzer.py
 scarletio/utils/async_utils.py
 scarletio/utils/base_method.py
 scarletio/utils/code.py
 scarletio/utils/compact.py
+scarletio/utils/dict_iterator_bases.py
 scarletio/utils/dict_update_iterable_iterator.py
 scarletio/utils/docs.py
 scarletio/utils/export_include.py
 scarletio/utils/function_tools.py
 scarletio/utils/hybrid_value_dictionary.py
 scarletio/utils/ignore_case_multi_value_dictionary.py
 scarletio/utils/ignore_case_string.py
@@ -88,14 +89,15 @@
 scarletio/utils/type_methodizer.py
 scarletio/utils/type_modulizer.py
 scarletio/utils/utils.py
 scarletio/utils/weak_core.py
 scarletio/utils/weak_item_dictionary.py
 scarletio/utils/weak_key_dictionary.py
 scarletio/utils/weak_map.py
+scarletio/utils/weak_set.py
 scarletio/utils/weak_value_dictionary.py
 scarletio/web_common/__init__.py
 scarletio/web_common/compressors.py
 scarletio/web_common/cookiejar.py
 scarletio/web_common/exceptions.py
 scarletio/web_common/formdata.py
 scarletio/web_common/header_building_and_parsing.py
```

### Comparing `scarletio-1.0.8/setup.py` & `scarletio-1.0.9/setup.py`

 * *Files identical despite different names*

