# Comparing `tmp/je_api_testka_dev-0.0.92.tar.gz` & `tmp/je_api_testka_dev-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka_dev-0.0.92.tar", last modified: Wed May 31 06:07:50 2023, max compression
+gzip compressed data, was "je_api_testka_dev-0.0.94.tar", last modified: Tue Jun 13 08:04:36 2023, max compression
```

## Comparing `je_api_testka_dev-0.0.92.tar` & `je_api_testka_dev-0.0.94.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.667583 je_api_testka_dev-0.0.92/
--rw-rw-rw-   0        0        0     3074 2023-05-31 06:07:50.666583 je_api_testka_dev-0.0.92/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.92/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.479880 je_api_testka_dev-0.0.92/je_api_testka/
--rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.92/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.92/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.487907 je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     5026 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     2615 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.491905 je_api_testka_dev-0.0.92/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.496966 je_api_testka_dev-0.0.92/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.502905 je_api_testka_dev-0.0.92/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     3497 2023-05-29 03:22:33.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.512681 je_api_testka_dev-0.0.92/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.521729 je_api_testka_dev-0.0.92/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     5456 2023-05-29 03:21:49.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.526858 je_api_testka_dev-0.0.92/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.539047 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     9028 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     4017 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     1688 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.545046 je_api_testka_dev-0.0.92/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.548046 je_api_testka_dev-0.0.92/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.553132 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.559050 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.565056 je_api_testka_dev-0.0.92/je_api_testka/utils/mock_server/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/mock_server/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/mock_server/flask_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.570140 je_api_testka_dev-0.0.92/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3346 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.576051 je_api_testka_dev-0.0.92/je_api_testka/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/__init__.py
--rw-rw-rw-   0        0        0     2982 2023-04-18 02:25:34.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.585618 je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.596571 je_api_testka_dev-0.0.92/je_api_testka/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0     6250 2023-05-31 06:04:47.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.602574 je_api_testka_dev-0.0.92/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2490 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.609577 je_api_testka_dev-0.0.92/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.612659 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.618572 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.626672 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.662573 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0     3074 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1170 2023-05-31 06:07:28.000000 je_api_testka_dev-0.0.92/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 06:07:50.668581 je_api_testka_dev-0.0.92/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.802329 je_api_testka_dev-0.0.94/
+-rw-rw-rw-   0        0        0     3074 2023-06-13 08:04:36.800084 je_api_testka_dev-0.0.94/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.94/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.480765 je_api_testka_dev-0.0.94/je_api_testka/
+-rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.94/je_api_testka/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.94/je_api_testka/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.505652 je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     5734 2023-06-13 07:24:00.000000 je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     3116 2023-06-13 07:15:23.000000 je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.512529 je_api_testka_dev-0.0.94/je_api_testka/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.523603 je_api_testka_dev-0.0.94/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/assert_result/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/assert_result/result_check.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.531758 je_api_testka_dev-0.0.94/je_api_testka/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     3497 2023-05-29 03:22:33.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.542815 je_api_testka_dev-0.0.94/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.551925 je_api_testka_dev-0.0.94/je_api_testka/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     5993 2023-06-13 07:58:24.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.561495 je_api_testka_dev-0.0.94/je_api_testka/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.594701 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     9231 2023-06-13 07:24:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/html_report_generate.py
+-rw-rw-rw-   0        0        0     4291 2023-06-13 07:30:18.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/json_report.py
+-rw-rw-rw-   0        0        0     2092 2023-06-13 07:34:49.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/xml_report.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.607234 je_api_testka_dev-0.0.94/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.610774 je_api_testka_dev-0.0.94/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.619739 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.636553 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.643569 je_api_testka_dev-0.0.94/je_api_testka/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-06-13 06:12:30.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.654741 je_api_testka_dev-0.0.94/je_api_testka/utils/mock_server/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/mock_server/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-06-13 08:03:10.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/mock_server/flask_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.670347 je_api_testka_dev-0.0.94/je_api_testka/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3589 2023-06-13 08:01:42.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.684243 je_api_testka_dev-0.0.94/je_api_testka/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     2982 2023-04-18 02:25:34.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.698253 je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.710058 je_api_testka_dev-0.0.94/je_api_testka/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     6250 2023-05-31 06:04:47.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.722720 je_api_testka_dev-0.0.94/je_api_testka/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2490 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/socket_server/api_testka_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.729638 je_api_testka_dev-0.0.94/je_api_testka/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.732636 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.743568 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.754361 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.796565 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0     3074 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2636 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1170 2023-06-13 08:04:12.000000 je_api_testka_dev-0.0.94/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 08:04:36.803342 je_api_testka_dev-0.0.94/setup.cfg
```

### Comparing `je_api_testka_dev-0.0.92/PKG-INFO` & `je_api_testka_dev-0.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_api_testka_dev
-Version: 0.0.92
+Version: 0.0.94
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.92/README.md` & `je_api_testka_dev-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/__init__.py` & `je_api_testka_dev-0.0.94/je_api_testka/__init__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/__main__.py` & `je_api_testka_dev-0.0.94/je_api_testka/__main__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/request_method.py` & `je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/request_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from je_api_testka.utils.exception.exception_tags import patch_error_message
 from je_api_testka.utils.exception.exception_tags import post_error_message
 from je_api_testka.utils.exception.exception_tags import put_error_message
 from je_api_testka.utils.exception.exception_tags import session_error_message
 from je_api_testka.utils.exception.exceptions import APITesterExecuteException
 from je_api_testka.utils.exception.exceptions import APITesterGetDataException
 from je_api_testka.utils.get_data_strcture.get_api_data import get_api_response_data
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.test_record.test_record_class import test_record_instance
 
 exception_message_dict = {
     "get": get_error_message,
     "put": put_error_message,
     "delete": delete_error_message,
     "post": post_error_message,
@@ -68,14 +69,20 @@
     :param test_url:
     :param soap:
     :param record_request_info:
     :param clean_record:
     :param result_check_dict:
     :param kwargs:
     """
+    apitestka_logger.info(
+        f"test_api_method, http_method: {http_method}, test_url:{test_url}, soap: {soap}, "
+        f"record_request_info: {record_request_info}, clean_record: {clean_record}, "
+        f"result_check_dict: {result_check_dict}, verify: {verify}, timeout: {timeout}, "
+        f"allow_redirects: {allow_redirects}"
+    )
     try:
         start_time: datetime = datetime.now()
         if soap is False:
             response = api_tester_method(http_method, test_url=test_url, verify=verify, timeout=timeout,
                                          allow_redirects=allow_redirects, **kwargs)
         else:
             headers = CaseInsensitiveDict()
@@ -91,18 +98,21 @@
                 test_record_instance.test_record_list.append(response_data)
             return {"response": response, "response_data": response_data}
         else:
             check_result(response_data, result_check_dict)
             if record_request_info:
                 test_record_instance.test_record_list.append(response_data)
             return {"response": response, "response_data": response_data}
-    except APITesterExecuteException as error:
-        raise repr(error)
     except Exception as error:
-        print(repr(error), file=sys.stderr)
+        apitestka_logger.error(
+            f"test_api_method, http_method: {http_method}, test_url:{test_url}, soap: {soap}, "
+            f"record_request_info: {record_request_info}, clean_record: {clean_record}, "
+            f"result_check_dict: {result_check_dict}, verify: {verify}, timeout: {timeout}, "
+            f"allow_redirects: {allow_redirects}, failed: {repr(error)}"
+        )
         test_record_instance.error_record_list.append([
             {
                 "http_method": http_method,
                 "test_url": test_url,
                 "soap": soap,
                 "record_request_info": record_request_info,
                 "clean_record": clean_record,
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/requests_http_method_wrapper.py` & `je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/requests_http_method_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import sys
-
 import requests
 from requests import Session
 from requests import delete
 from requests import get
 from requests import head
 from requests import options
 from requests import patch
 from requests import post
 from requests import put
 
 from je_api_testka.utils.exception.exception_tags import http_method_have_wrong_type
 from je_api_testka.utils.exception.exception_tags import wrong_http_method_error_message
 from je_api_testka.utils.exception.exceptions import APITesterException
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 
 _session = Session()
 
 http_method_dict = {
     "get": get,
     "put": put,
     "patch": patch,
@@ -40,21 +39,26 @@
 ]:
     """
     :param http_method: what http method we use to api test
     :return: one of method in http_method_dict if not exists will raise exception
     """
     try:
         if not isinstance(http_method, str):
+            apitestka_logger.error(
+                f"get_http_method failed. {APITesterException(wrong_http_method_error_message)}")
             raise APITesterException(wrong_http_method_error_message)
         http_method = str(http_method).lower()
         if http_method not in http_method_dict:
+            apitestka_logger.error(
+                f"get_http_method failed. {APITesterException(http_method_have_wrong_type)}")
             raise APITesterException(http_method_have_wrong_type)
         return http_method_dict.get(http_method)
     except APITesterException as error:
-        print(repr(error), file=sys.stderr)
+        apitestka_logger.error(
+            f"get_http_method failed. {repr(error)}")
 
 
 def api_tester_method(http_method: str, test_url: str, verify: bool = False, timeout: int = 5,
                       allow_redirects: bool = False, **kwargs) -> requests.Response:
     """
     :param http_method: what http method we use to api test
     :param test_url: what url we want to test
@@ -62,11 +66,13 @@
     :param verify: this connect need verify or not
     :param timeout: timeout sec
     :param allow_redirects: allow to redirects to another request
     :return: test response
     """
     response = get_http_method(http_method)
     if response is None:
+        apitestka_logger.error(
+            f"api_tester_method failed. {APITesterException(wrong_http_method_error_message)}")
         raise APITesterException(wrong_http_method_error_message)
     else:
         response = response(test_url, verify=verify, timeout=timeout, allow_redirects=allow_redirects, **kwargs)
     return response
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/assert_result/result_check.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/assert_result/result_check.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/callback/callback_function_executor.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/exception/exception_tags.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/exception/exceptions.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/executor/action_executor.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/executor/action_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from je_api_testka.utils.generate_report.html_report_generate import generate_html
 from je_api_testka.utils.generate_report.html_report_generate import generate_html_report
 from je_api_testka.utils.generate_report.json_report import generate_json
 from je_api_testka.utils.generate_report.json_report import generate_json_report
 from je_api_testka.utils.generate_report.xml_report import generate_xml
 from je_api_testka.utils.generate_report.xml_report import generate_xml_report
 from je_api_testka.utils.json.json_file.json_file import read_action_json
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.mock_server.flask_mock_server import flask_mock_server_instance
 from je_api_testka.utils.package_manager.package_manager_class import package_manager
 
 
 class Executor(object):
 
     def __init__(self):
@@ -27,18 +28,20 @@
             "test_api_method": test_api_method,
             "generate_html": generate_html,
             "generate_html_report": generate_html_report,
             "generate_json": generate_json,
             "generate_json_report": generate_json_report,
             "generate_xml": generate_xml,
             "generate_xml_report": generate_xml_report,
-            # execute
+            # Execute
             "execute_action": self.execute_action,
             "execute_files": self.execute_files,
+            # Add package
             "add_package_to_executor": package_manager.add_package_to_executor,
+            "add_package_to_callback_executor": package_manager.add_package_to_callback_executor,
             # mock
             "flask_mock_server_add_router": flask_mock_server_instance.add_router,
             "start_flask_mock_server": flask_mock_server_instance.start_mock_server,
         }
         # get all builtin function and add to event dict
         for function in getmembers(builtins, isbuiltin):
             self.event_dict.update({str(function[0]): function[1]})
@@ -63,46 +66,50 @@
         [
             ["method on event_dict", {"param": params}],
             ["method on event_dict", {"param": params}]
         ]
         for loop and use execute_event function to execute
         :return: recode string, response as list
         """
+        apitestka_logger.info(f"execute_action, action_list: {action_list}")
         if isinstance(action_list, dict):
             action_list: list = action_list.get("api_testka", None)
             if action_list is None:
                 raise APITesterExecuteException(executor_list_error)
         execute_record_dict = dict()
         try:
             if len(action_list) > 0 or isinstance(action_list, list) is False:
                 pass
             else:
                 raise APITesterExecuteException(executor_list_error)
         except Exception as error:
-            print(repr(error), file=sys.stderr)
+            apitestka_logger.info(f"execute_action, action_list: {action_list}, "
+                                  f"failed: {repr(error)}")
         for action in action_list:
             try:
                 event_response = self._execute_event(action)
                 execute_record: str = "execute: " + str(action)
                 execute_record_dict.update({execute_record: event_response})
             except Exception as error:
-                print(repr(error), file=sys.stderr)
-                print(action, file=sys.stderr)
+                apitestka_logger.info(
+                    f"execute_action, action_list: {action_list}, "
+                    f"action: {action}, failed: {repr(error)}")
                 execute_record = "execute: " + str(action)
                 execute_record_dict.update({execute_record: repr(error)})
         for key, value in execute_record_dict.items():
             print(key)
             print(value)
         return execute_record_dict
 
     def execute_files(self, execute_files_list: list) -> typing.List[typing.Any]:
         """
         :param execute_files_list: list include execute files path
         :return: every execute detail as list
         """
+        apitestka_logger.info(f"execute_files, execute_files_list: {execute_files_list}")
         execute_detail_list: list = list()
         for file in execute_files_list:
             execute_detail_list.append(self.execute_action(read_action_json(file)))
         return execute_detail_list
 
 
 executor = Executor()
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/file_process/get_dir_file_list.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/html_report_generate.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/html_report_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import typing
 from threading import Lock
 
 from je_api_testka.utils.exception.exception_tags import html_generate_no_data_tag
 from je_api_testka.utils.exception.exceptions import APIHTMLException
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.test_record.test_record_class import test_record_instance
 
 lock = Lock()
 
 _html_string_head = \
     """
     <!DOCTYPE html>
@@ -198,14 +199,15 @@
     """.strip()
 
 
 def generate_html() -> typing.Tuple[list, list]:
     """
     :return: test success_list & test failure_list
     """
+    apitestka_logger.info(f"generate_html")
     if len(test_record_instance.test_record_list) == 0 and len(test_record_instance.error_record_list) == 0:
         raise APIHTMLException(html_generate_no_data_tag)
     else:
         success_list: list = list()
         for record_data in test_record_instance.test_record_list:
             success_list.append(
                 _success_table.format(
@@ -245,14 +247,15 @@
 
 
 def generate_html_report(html_file_name: str = "default_name") -> None:
     """
     :param html_file_name: save html file name
     :return:
     """
+    apitestka_logger.info(f"generate_html_report html_file_name:{html_file_name}")
     success_list, failure_list = generate_html()
     try:
         lock.acquire()
         with open(html_file_name + ".html", "w+") as file_to_write:
             file_to_write.writelines(
                 _html_string_head
             )
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/json_report.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/json_report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
 import sys
 import typing
 from threading import Lock
 
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.test_record.test_record_class import test_record_instance
 from je_api_testka.utils.exception.exception_tags import cant_save_json_report_record_us_null
 from je_api_testka.utils.exception.exceptions import APIJsonReportException
 
 
 def generate_json() -> typing.Tuple[dict, dict]:
     """
     :return: test success_dict test failure_dict
     """
+    apitestka_logger.info("generate_json")
     if len(test_record_instance.test_record_list) == 0 and len(test_record_instance.error_record_list) == 0:
         raise APIJsonReportException(cant_save_json_report_record_us_null)
     else:
         success_dict = dict()
         success_count: int = 1
         success_test_str: str = "Success_Test"
         for record_data in test_record_instance.test_record_list:
@@ -64,25 +66,26 @@
         return success_dict, failure_dict
 
 
 def generate_json_report(json_file_name: str = "default_name") -> None:
     """
     :param json_file_name: save json file's name
     """
+    apitestka_logger.info(f"generate_json_report, json_file_name: {json_file_name}")
     lock = Lock()
     success_dict, failure_dict = generate_json()
     try:
         lock.acquire()
         with open(json_file_name + "_failure.json", "w+") as file_to_write:
             json.dump(dict(failure_dict), file_to_write, indent=4)
     except Exception as error:
-        print(repr(error), file=sys.stderr)
+        apitestka_logger.error(f"generate_json_report, failed: {repr(error)}")
     finally:
         lock.release()
     try:
         lock.acquire()
         with open(json_file_name + "_success.json", "w+") as file_to_write:
             json.dump(dict(success_dict), file_to_write, indent=4)
     except Exception as error:
-        print(repr(error), file=sys.stderr)
+        apitestka_logger.error(f"generate_json_report, failed: {repr(error)}")
     finally:
         lock.release()
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/xml_report.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/xml_report.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 import sys
 import typing
 from threading import Lock
 from xml.dom.minidom import parseString
 
 from je_api_testka.utils.generate_report.json_report import generate_json
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.xml.change_xml_structure.change_xml_structure import dict_to_elements_tree
 
 
 def generate_xml() -> typing.Tuple[str, str]:
     """
     :return: success_xml_string, failure_xml_string
     """
+    apitestka_logger.info("generate_xml")
     success_dict, failure_dict = generate_json()
     success_dict = dict({"xml_data": success_dict})
     failure_dict = dict({"xml_data": failure_dict})
     success_json_to_xml = dict_to_elements_tree(success_dict)
     failure_json_to_xml = dict_to_elements_tree(failure_dict)
     return success_json_to_xml, failure_json_to_xml
 
 
 def generate_xml_report(xml_file_name: str = "default_name") -> None:
     """
     :param xml_file_name: save xml file with xml_file_name
     """
+    apitestka_logger.info(f"generate_xml_report, xml_file_name: {xml_file_name}")
     success_xml, failure_xml = generate_xml()
     success_xml = parseString(success_xml)
     failure_xml = parseString(failure_xml)
     success_xml = success_xml.toprettyxml()
     failure_xml = failure_xml.toprettyxml()
     lock = Lock()
     try:
         lock.acquire()
         with open(xml_file_name + "_failure.xml", "w+") as file_to_write:
             file_to_write.write(failure_xml)
     except Exception as error:
-        print(repr(error), file=sys.stderr)
+        apitestka_logger.error(f"generate_xml_report, xml_file_name: {xml_file_name}, "
+                               f"failed: {repr(error)}")
     finally:
         lock.release()
     try:
         lock.acquire()
         with open(xml_file_name + "_success.xml", "w+") as file_to_write:
             file_to_write.write(success_xml)
             pass
     except Exception as error:
-        print(repr(error), file=sys.stderr)
+        apitestka_logger.error(f"generate_xml_report, xml_file_name: {xml_file_name}, "
+                               f"failed: {repr(error)}")
     finally:
         lock.release()
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/get_data_strcture/get_api_data.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/get_data_strcture/get_api_data.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_format/json_process.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/mock_server/flask_mock_server.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/mock_server/flask_mock_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing
 
 from flask.app import Flask
 
 from je_api_testka.utils.exception.exception_tags import get_bad_api_router_setting
 from je_api_testka.utils.exception.exceptions import MockServerException
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 
 
 class FlaskMockServer(object):
     pass
 
     def __init__(self, host, port):
         """
@@ -24,24 +25,32 @@
 
     def add_router(self, rule_and_function_dict: dict, **kwargs) -> None:
         """
         :param rule_and_function_dict: dict include {"rule(path): function"}
         :param kwargs: use to set methods or another param
         :return:
         """
+        apitestka_logger.info(
+            f"add_router, rule_and_function_dict: {rule_and_function_dict}, params: {kwargs}"
+        )
         for rule, function in rule_and_function_dict.items():
             if isinstance(rule, str) and isinstance(function, typing.Callable):
                 self.app.route(rule, **kwargs)(function)
             else:
+                apitestka_logger.error(
+                    f"add_router, rule_and_function_dict: {rule_and_function_dict}, params: {kwargs}, "
+                    f"failed: {MockServerException(get_bad_api_router_setting)}"
+                )
                 raise MockServerException(get_bad_api_router_setting)
 
     def start_mock_server(self) -> None:
         """
         start mock server
         """
+        apitestka_logger.info(f"start_mock_server")
         self.add_router(
             {"/": self.api_testka_index_function},
             methods=["GET"]
         )
         self.app.run(self.host, self.port)
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/package_manager/package_manager_class.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/package_manager/package_manager_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import typing
 from importlib import import_module
 from importlib.util import find_spec
 from inspect import getmembers, isfunction, isbuiltin, isclass
 from sys import stderr
 
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
+
 
 class PackageManager(object):
 
     def __init__(self):
         self.installed_package_dict = {
         }
         self.executor = None
@@ -29,23 +31,25 @@
                     print(repr(error), file=stderr)
         return self.installed_package_dict.get(package, None)
 
     def add_package_to_executor(self, package):
         """
         :param package: package's function will add to executor
         """
+        apitestka_logger.info(f"add_package_to_executor, package: {package}")
         self.add_package_to_target(
             package=package,
             target=self.executor
         )
 
     def add_package_to_callback_executor(self, package) -> None:
         """
         :param package: package's function will add to callback_executor
         """
+        apitestka_logger.info(f"add_package_to_callback_executor, package: {package}")
         self.add_package_to_target(
             package=package,
             target=self.callback_executor
         )
 
     def get_member(self, package, predicate, target) -> None:
         """
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/project/create_project_structure.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/project/create_project_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/template_executor.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/template_keyword.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/template_keyword.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/scheduler/extend_apscheduler.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/scheduler/extend_apscheduler.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/socket_server/api_testka_socket_server.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/socket_server/api_testka_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.94/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/PKG-INFO` & `je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-api-testka-dev
-Version: 0.0.92
+Version: 0.0.94
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/SOURCES.txt` & `je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 je_api_testka/utils/get_data_strcture/__init__.py
 je_api_testka/utils/get_data_strcture/get_api_data.py
 je_api_testka/utils/json/__init__.py
 je_api_testka/utils/json/json_file/__init__.py
 je_api_testka/utils/json/json_file/json_file.py
 je_api_testka/utils/json/json_format/__init__.py
 je_api_testka/utils/json/json_format/json_process.py
+je_api_testka/utils/logging/__init__.py
+je_api_testka/utils/logging/loggin_instance.py
 je_api_testka/utils/mock_server/__init__.py
 je_api_testka/utils/mock_server/flask_mock_server.py
 je_api_testka/utils/package_manager/__init__.py
 je_api_testka/utils/package_manager/package_manager_class.py
 je_api_testka/utils/project/__init__.py
 je_api_testka/utils/project/create_project_structure.py
 je_api_testka/utils/project/template/__init__.py
```

### Comparing `je_api_testka_dev-0.0.92/pyproject.toml` & `je_api_testka_dev-0.0.94/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_api_testka_dev"
-version = "0.0.92"
+version = "0.0.94"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Requests Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

