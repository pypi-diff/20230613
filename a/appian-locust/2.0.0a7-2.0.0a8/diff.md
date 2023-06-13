# Comparing `tmp/appian-locust-2.0.0a7.tar.gz` & `tmp/appian-locust-2.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0a7.tar", last modified: Fri Jun  9 16:15:02 2023, max compression
+gzip compressed data, was "appian-locust-2.0.0a8.tar", last modified: Tue Jun 13 20:35:12 2023, max compression
```

## Comparing `appian-locust-2.0.0a7.tar` & `appian-locust-2.0.0a8.tar`

### file list

```diff
@@ -1,57 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:15:02.535519 appian-locust-2.0.0a7/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5403 2023-06-09 16:15:02.535519 appian-locust-2.0.0a7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:15:02.534519 appian-locust-2.0.0a7/appian_locust/
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2479 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6282 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_design.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_feature_toggle_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_grid_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    51994 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)     5171 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_locust_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7789 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_portals.py
--rw-rw-rw-   0 root         (0) root         (0)    16614 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_records.py
--rw-rw-rw-   0 root         (0) root         (0)     7380 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_records_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7464 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_save_request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     9934 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_sites.py
--rw-rw-rw-   0 root         (0) root         (0)     4514 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_task_opener.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_ui_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/actions_info.py
--rw-rw-rw-   0 root         (0) root         (0)    14940 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/appianclient.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/application.py
--rw-rw-rw-   0 root         (0) root         (0)     3950 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/application_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/design_object.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/design_object_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/design_object_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/design_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/feature_flag.py
--rw-rw-rw-   0 root         (0) root         (0)    16346 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     1431 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/loadDriverUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/news_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/record_list_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/record_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/records_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/reports_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/site_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/site_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     1261 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/sites_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/tasks_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2211 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/tempo_navigator.py
--rw-rw-rw-   0 root         (0) root         (0)    73573 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/uiform.py
--rw-rw-rw-   0 root         (0) root         (0)    15051 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:15:02.535519 appian-locust-2.0.0a7/appian_locust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5403 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1521 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-09 16:15:02.535519 appian-locust-2.0.0a7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.259654 appian-locust-2.0.0a8/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5449 2023-06-13 20:35:12.259654 appian-locust-2.0.0a8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.254654 appian-locust-2.0.0a8/appian_locust/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9592 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2498 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_design.py
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_feature_toggle_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7849 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_grid_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    52246 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_locust_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7747 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_portals.py
+-rw-rw-rw-   0 root         (0) root         (0)    16611 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     7390 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_records_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7474 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_save_request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9939 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_sites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_task_opener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_ui_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)    16940 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/appianclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.255654 appian-locust-2.0.0a8/appian_locust/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/exceptions/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/feature_flag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.256654 appian-locust-2.0.0a8/appian_locust/info/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/actions_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/news_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/records_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/reports_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/sites_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/tasks_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.257654 appian-locust-2.0.0a8/appian_locust/objects/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/application.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/design_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/page.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/site.py
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/system_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.258654 appian-locust-2.0.0a8/appian_locust/uiform/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/application_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/design_object_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/design_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/record_list_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/record_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)    73478 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/uiform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.259654 appian-locust-2.0.0a8/appian_locust/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16347 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/utilities/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1393 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/utilities/loadDriverUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/utilities/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    14863 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.254654 appian-locust-2.0.0a8/appian_locust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5449 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-13 20:35:12.259654 appian-locust-2.0.0a8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/setup.py
```

### Comparing `appian-locust-2.0.0a7/LICENSE` & `appian-locust-2.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a7/PKG-INFO` & `appian-locust-2.0.0a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a7
+Version: 2.0.0a8
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -75,15 +75,15 @@
     [pipenv]
     allow_prereleases = true
 
 2. Configure your test to point at the Appian instance you will be using.
 You can use example file provided in this repository `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_:
 
 - Set ``host_address`` to the address of your Appian instance.
-- In ``auth``, specify the username and password of the user account to use.
+- In ``auth``, specify the username and password of the user account to use. Note: This user must be able to access Tempo.
 
 .. code-block:: json
 
     {
         "host_address": "site-name.appiancloud.com",
         "auth": [
             "user.name",
```

### Comparing `appian-locust-2.0.0a7/README.rst` & `appian-locust-2.0.0a8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     [pipenv]
     allow_prereleases = true
 
 2. Configure your test to point at the Appian instance you will be using.
 You can use example file provided in this repository `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_:
 
 - Set ``host_address`` to the address of your Appian instance.
-- In ``auth``, specify the username and password of the user account to use.
+- In ``auth``, specify the username and password of the user account to use. Note: This user must be able to access Tempo.
 
 .. code-block:: json
 
     {
         "host_address": "site-name.appiancloud.com",
         "auth": [
             "user.name",
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_actions.py` & `appian-locust-2.0.0a8/appian_locust/_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, Optional
 
 from requests.models import Response
 
-from . import logger
+from .utilities import logger
 from ._base import _Base
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error
-from .helper import format_label
+from .utilities.helper import format_label
 from .uiform import SailUiForm
 
 log = logger.getLogger(__name__)
 
 ACTIONS_ALL_PATH = "/suite/api/tempo/open-a-case/available-actions?ids=%5B%5D"
 ACTIONS_FEED_PATH = "/suite/api/feed/tempo?m=menu-actions&c=0"
 ACTIONS_INTERFACE_PATH = "/suite/rest/a/sites/latest/D6JMim/pages/actions/interface"
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_admin.py` & `appian-locust-2.0.0a8/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a7/appian_locust/_base.py` & `appian-locust-2.0.0a8/appian_locust/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .helper import list_filter
-from . import logger
+from .utilities.helper import list_filter
+from .utilities import logger
 from typing import Any, Optional
 
 
 log = logger.getLogger(__name__)
 
 
 class _Base():
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_design.py` & `appian-locust-2.0.0a8/appian_locust/_design.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, Optional
 
 from ._interactor import _Interactor
 from ._locust_error_handler import raises_locust_error
-from .design_object import DesignObject
-from .helper import find_component_by_label_and_type_dict, find_component_by_type_and_attribute_and_index_in_dict, find_component_by_attribute_in_dict
+from .objects import DesignObject
+from .utilities.helper import find_component_by_label_and_type_dict, find_component_by_type_and_attribute_and_index_in_dict, find_component_by_attribute_in_dict
 from .uiform import SailUiForm
 
 DESIGN_URI_PATH: str = "/suite/rest/a/applications/latest/app/design"
 
 
 def get_available_design_objects(state: Dict[str, Any]) -> Dict[str, DesignObject]:
     name_column = find_component_by_label_and_type_dict(type="GridFieldColumn", attribute="label", value="Name",
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.0a8/appian_locust/_feature_toggle_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Tuple, Optional, Generator, Callable
 
 from locust.clients import HttpSession
 
 from .feature_flag import FeatureFlag
 from ._interactor import _Interactor
 from ._locust_error_handler import test_response_for_error
-from .logger import getLogger
+from .utilities.logger import getLogger
 
 log = getLogger(__name__)
 
 
 def get_client_feature_toggles(interactor: _Interactor, session: HttpSession) -> Tuple[str, str]:
     """
     Given an authenticated user, recover the feature toggles from the minified javascript
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_grid_interactor.py` & `appian-locust-2.0.0a8/appian_locust/_grid_interactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, List, Optional
 
-from .helper import extract_values_multiple_key_values, find_component_by_label_and_type_dict
+from .utilities.helper import extract_values_multiple_key_values, find_component_by_label_and_type_dict
 
-from . import logger
+from .utilities import logger
 
 log = logger.getLogger(__name__)
 
 
 class GridInteractor:
     """
     Set of utility methods for interacting with grids, i.e. finding them, and manipulating them
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_interactor.py` & `appian-locust-2.0.0a8/appian_locust/_interactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,50 +6,52 @@
 from datetime import date, datetime
 from re import match, search
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 from locust.clients import HttpSession, ResponseContextManager
 from requests import Response
 
-from . import logger
+from .utilities import logger
 from ._locust_error_handler import log_locust_error, test_response_for_error
 from ._save_request_builder import save_builder
 from .exceptions import BadCredentialsException, MissingCsrfTokenException, ComponentNotFoundException
-from .helper import find_component_by_attribute_in_dict, get_username
+from .utilities.helper import find_component_by_attribute_in_dict, get_username
 from ._records_helper import get_url_stub_from_record_list_post_request_url
 
 log = logger.getLogger(__name__)
 
 # TODO: Consider breaking this class up into smaller pieces
 
 
 RECORD_PATH = "recorded_responses"
 
 
 class _Interactor:
-    def __init__(self, session: HttpSession, host: str, portals_mode: bool = False) -> None:
+    def __init__(self, session: HttpSession, host: str, portals_mode: bool = False, request_timeout: int = 300) -> None:
         """
         Class that represents interactions with the UI and Appian system
         If you want to record all requests made, you can set the record_mode attribute
         on the client, see the mock_client.py in the tests directory as an example
 
         >>> setattr(self.client, 'record_mode', True)
 
         Args:
             session: Locust session/client object
             host (str): Host URL inherited from subclass to conform with Mypy standards
             portals_mode (bool): Set to true if attempting to connect to a portals site
+            request_timeout (int): time in seconds after which requests initiated by the Interactor should time out
         """
         self.client = session
         self.host = host
         self.record_mode = True if hasattr(self.client, "record_mode") else False
         self.datatype_cache = DataTypeCache()
         self.user_agent = ""
         self.portals_mode = portals_mode
         self.url_pattern_version = 0
+        self.__request_timeout = request_timeout
         # Set to default as desktop request.
         self.set_user_agent_to_desktop()
 
     # GENERIC UTILITY METHODS
     def set_user_agent_to_desktop(self) -> None:
         self.user_agent = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/61.0.3163.100 Safari/537.36"
 
@@ -147,15 +149,15 @@
         elif isinstance(payload, dict):
             post_payload = json.dumps(payload).encode()
         elif isinstance(payload, str):
             post_payload = payload.encode()
         else:
             log_locust_error(Exception("Cannot POST a payload that is not of type dict or string"))
             sys.exit(1)
-        with self.client.post(uri, data=post_payload, headers=headers, timeout=60, name=label, files=files,
+        with self.client.post(uri, data=post_payload, headers=headers, timeout=self.__request_timeout, name=label, files=files,
                               catch_response=True) as resp:  # type: ResponseContextManager
             try:
                 test_response_for_error(resp, uri, raise_error=check_login, username=username)
             except Exception as e:
                 raise e
             else:
                 if check_login:
@@ -255,15 +257,15 @@
             else:
                 headers = self.setup_request_headers(uri)
         kwargs: Dict[str, Any] = {'name': label, 'catch_response': True}
 
         uri = self.replace_base_path_if_appropriate(uri)
         if headers is not None:
             kwargs['headers'] = headers
-            kwargs['timeout'] = 60
+            kwargs['timeout'] = self.__request_timeout
         with self.client.get(uri, **kwargs) as resp:  # type: ResponseContextManager
             if check_login and not self.portals_mode:
                 self.check_login(resp)
             if not self.portals_mode:
                 username = get_username(self.auth)
                 test_response_for_error(resp, uri, raise_error=check_login, username=username)
             if self.record_mode:
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.0a8/appian_locust/_locust_error_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from functools import wraps
 from typing import Any, Callable, Optional
 
 from locust.clients import ResponseContextManager
 from requests.exceptions import HTTPError
 from requests.models import Response
 
-from appian_locust.helper import ENV
+from .utilities.helper import ENV
 
-from . import logger
+from .utilities import logger
 
 log = logger.getLogger(__name__)
 
 
 def _format_http_error(resp: Response, uri: str, username: str) -> str:
     """Taken from Response.raise_for_status. Formats the http error message,
      additionally adding the username
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_news.py` & `appian-locust-2.0.0a8/appian_locust/_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, Tuple, Optional
 
-from appian_locust import logger
-from appian_locust._base import _Base
-from appian_locust._interactor import _Interactor
-from appian_locust._locust_error_handler import log_locust_error
+from .utilities import logger
+from ._base import _Base
+from ._interactor import _Interactor
+from ._locust_error_handler import log_locust_error
 
 log = logger.getLogger(__name__)
 
 NEWS_FEED_PATH = "/suite/api/feed/tempo?t=e,x,b&m=menu-news&st=o"
 NEWS_NAV_PATH = ["/suite/rest/a/sites/latest/D6JMim/page/", "news", "/nav"]
 NEWS_SEARCH_PATH = "/suite/api/feed/tempo?q="
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_portals.py` & `appian-locust-2.0.0a8/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a7/appian_locust/_records.py` & `appian-locust-2.0.0a8/appian_locust/_records.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import random
 from typing import Any, Dict, Tuple, Optional
 from urllib.parse import quote
 
 import requests
 
-from appian_locust import logger
+from .utilities import logger
 
 from ._base import _Base
 from ._interactor import _Interactor
 from ._records_helper import (get_all_records_from_json,
                               get_all_record_types_from_json, get_records_from_json_by_column)
 from ._locust_error_handler import log_locust_error
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_records_helper.py` & `appian-locust-2.0.0a8/appian_locust/_records_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import Any, Dict, Tuple, Optional
 
 from ._locust_error_handler import log_locust_error
-from .helper import extract_values, find_component_by_attribute_in_dict
+from .utilities.helper import extract_values, find_component_by_attribute_in_dict
 from re import match
 
 
 def get_all_record_types_from_json(json_response: Dict[str, Any]) -> Dict[str, Any]:
     response = dict()
     for current_record_type in json_response["ui"]["contents"][0]["feedItems"]:
         title = current_record_type['title'].strip()
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_reports.py` & `appian-locust-2.0.0a8/appian_locust/_reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Optional
 from urllib.parse import quote
 
 from ._base import _Base
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error, test_response_for_error
-from .helper import format_label
+from .utilities.helper import format_label
 from .uiform import SailUiForm
 
 ALL_REPORTS_URI = "/suite/rest/a/uicontainer/latest/reports"
 REPORTS_INTERFACE_PATH = "/suite/rest/a/sites/latest/D6JMim/pages/reports/interface"
 REPORTS_LINK_PATH = ["/suite/rest/a/sites/latest/D6JMim/pages/reports/report/", "/reportlink"]
 REPORTS_NAV_PATH = ["/suite/rest/a/sites/latest/D6JMim/page/", "reports", "/nav"]
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_save_request_builder.py` & `appian-locust-2.0.0a8/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a7/appian_locust/_sites.py` & `appian-locust-2.0.0a8/appian_locust/_sites.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import enum
 import random
 from typing import Any, Dict, List, Union, Optional
 
-from . import logger
+from .utilities import logger
 from ._base import _Base
 from ._interactor import _Interactor
 from ._news import NEWS_NAV_PATH
-from .helper import extract_values, format_label
+from .utilities.helper import extract_values, format_label
 from ._records_helper import get_all_records_from_json
-from .site_objects import Site, Page, PageType
+from .objects import Site, Page, PageType
+from .exceptions import (PageNotFoundException,
+                         InvalidSiteException,
+                         SiteNotFoundException)
 
 log = logger.getLogger(__name__)
 
 SITES_NAV_PATH = ["/suite/rest/a/sites/latest/", "/page/", "/nav"]
 SITES_PAGE_PATH = ["/suite/rest/a/sites/latest/", "/pages/", "/"]
 
 
@@ -217,19 +220,7 @@
         headers["Accept"] = self.BROWSER_ACCEPT_HEADER
         return headers
 
     def _setup_headers_with_sail_json(self) -> dict:
         headers = self.interactor.setup_sail_headers()
         headers["Accept"] = "application/vnd.appian.tv.ui+json"
         return headers
-
-
-class SiteNotFoundException(Exception):
-    pass
-
-
-class PageNotFoundException(Exception):
-    pass
-
-
-class InvalidSiteException(Exception):
-    pass
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_task_opener.py` & `appian-locust-2.0.0a8/appian_locust/_task_opener.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, Optional
 
-from . import logger
+from .utilities import logger
 from ._interactor import _Interactor
-from .helper import find_component_by_attribute_in_dict
+from .utilities.helper import find_component_by_attribute_in_dict
 
 log = logger.getLogger(__name__)
 
 
 class _TaskOpener:
 
     def __init__(self, interactor: _Interactor) -> None:
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_tasks.py` & `appian-locust-2.0.0a8/appian_locust/_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Union, Optional
 
-from . import logger
+from .utilities import logger
 from ._base import _Base
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error
 from ._task_opener import _TaskOpener
 from .uiform import SailUiForm
 
 log = logger.getLogger(__name__)
```

### Comparing `appian-locust-2.0.0a7/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.0a8/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a7/appian_locust/actions_info.py` & `appian-locust-2.0.0a8/appian_locust/info/actions_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict
 
-from ._actions import _Actions
+from .._actions import _Actions
 
 
 class ActionsInfo:
 
     def __init__(self, actions: _Actions):
         self.__actions = actions
```

### Comparing `appian-locust-2.0.0a7/appian_locust/appianclient.py` & `appian-locust-2.0.0a8/appian_locust/appianclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 import uuid
 from typing import List, Tuple, Optional, Callable, Generator
 
 from locust import SequentialTaskSet, TaskSet
 from locust.clients import HttpSession
 from requests import Response
 
-from . import logger
+from .utilities import logger
 from .feature_flag import FeatureFlag
+from .utilities import loadDriverUtils, DEFAULT_CONFIG_PATH
 from ._feature_toggle_helper import (get_client_feature_toggles,
                                      override_default_feature_flags,
                                      set_mobile_feature_flags)
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error
 from .exceptions import MissingConfigurationException
 from ._actions import _Actions
+from ._news import _News
 from ._records import _Records
 from ._reports import _Reports
 from ._sites import _Sites
 from ._tasks import _Tasks
-from .tempo_navigator import TempoNavigator
 from .visitor import Visitor
-from .site_helper import SiteHelper
+from .system_operator import SystemOperator
+from .info import ActionsInfo, NewsInfo, RecordsInfo, ReportsInfo, SitesInfo, TasksInfo
 
 log = logger.getLogger(__name__)
 
 
 # Can be called during an initalization event of a locust test to
 # procedurally generate Appian credentials
 def procedurally_generate_credentials(CONFIG: dict) -> None:
@@ -102,22 +104,14 @@
     return CONFIG['credentials']
 
 
 def _trim_trailing_slash(host: str) -> str:
     return host[:-1] if host and host.endswith('/') else host
 
 
-class NoOpEvents():
-    def fire(self, *args: str, **kwargs: int) -> None:
-        pass
-
-    def context(self, *args: str, **kwargs: int) -> dict:
-        return {}
-
-
 def appian_client_without_locust(host: str, record_mode: bool = False, base_path_override: Optional[str] = None) -> 'AppianClient':
     """
     Returns an AppianClient that can be used without locust to make requests against a host, e.g.
 
     >>> appian_client_without_locust()
     >>> client.login(auth=('username', 'password'))
     >>> client.get_client_feature_toggles()
@@ -129,68 +123,119 @@
     inner_client = HttpSession(_trim_trailing_slash(host), NoOpEvents(), NoOpEvents())
     if record_mode:
         setattr(inner_client, 'record_mode', True)
     return AppianClient(inner_client, host=host, base_path_override=base_path_override)
 
 
 class AppianClient:
-    def __init__(self, session: HttpSession, host: str, base_path_override: Optional[str] = None, portals_mode: bool = False) -> None:
+    def __init__(self, session: HttpSession, host: str, base_path_override: Optional[str] = None, portals_mode: bool = False,
+                 config_path: str = DEFAULT_CONFIG_PATH) -> None:
         """
         Appian client class contains all the required functions to interact with Tempo.
 
         Note: This class will be called inside ``AppianTaskSet`` so it is not necessary to call this explicitly in a test.
         ``self.appian`` can be used directly in a test.
 
         Args:
             session: Locust session/client object
             host (str): Host URL
+            base_path_override (str): override for sites where /suite is not the base path
+            config_path (str): path to configuration file
 
         """
         self.client = session
         self.portals_mode = portals_mode
         self.host = _trim_trailing_slash(host)
-        self._interactor = _Interactor(self.client, self.host, portals_mode=portals_mode)
-        actions = _Actions(self._interactor)
-        tasks = _Tasks(self._interactor)
-        reports = _Reports(self._interactor)
-        records = _Records(self._interactor)
-        sites = _Sites(self._interactor)
-
-        self._visitor = Visitor(self._interactor, tasks, reports, actions, records, sites)
-        self._site_helper = SiteHelper(self._interactor, actions)
-        self._tempo_navigator = TempoNavigator(self._interactor, tasks, reports, actions, records, sites)
+
+        timeout = 300
+        if os.path.exists(config_path):
+            config_timeout = loadDriverUtils().load_config(config_path).get('request_timeout', None)
+            if config_timeout:
+                log.info(f"Overriding default timeout to {config_timeout}s")
+                timeout = config_timeout
+
+        self._interactor = _Interactor(self.client, self.host, portals_mode=portals_mode, request_timeout=timeout)
+        self._news = _News(self._interactor)
+        self._actions = _Actions(self._interactor)
+        self._tasks = _Tasks(self._interactor)
+        self._reports = _Reports(self._interactor)
+        self._records = _Records(self._interactor)
+        self._sites = _Sites(self._interactor)
+
+        self._visitor = Visitor(self._interactor,
+                                self._tasks,
+                                self._reports,
+                                self._actions,
+                                self._records,
+                                self._sites)
+        self._system_operator = SystemOperator(self._interactor, self._actions)
 
         # Adding a few session specific attributes to self.client to that it can be carried and handled by session
         # in case of having multiple sessions in the future.
         setattr(self.client, "feature_flag", "")
         setattr(self.client, "feature_flag_extended", "")
 
         # Used for sites where /suite is not in the URL, i.e. local builds
         setattr(self.client, "base_path_override", base_path_override)
 
     @property
-    def visitor(self) -> Visitor:
+    def actions_info(self) -> ActionsInfo:
         """
-        Visitor that can be used to navigate to different types of pages in an Appian instance
+        Navigate to actions and gather information about available actions
         """
-        return self._visitor
+        return ActionsInfo(self._actions)
+
+    @property
+    def news_info(self) -> NewsInfo:
+        """
+        Navigate to news and fetch information on news entries
+        """
+        return NewsInfo(self._news)
 
     @property
-    def tempo_navigator(self) -> TempoNavigator:
+    def records_info(self) -> RecordsInfo:
         """
-        Tempo Navigator that can be used to fetch objects which can provide metadata about Tempo Tabs
+        Navigate to records and gather information about available records
         """
-        return self._tempo_navigator
+        return RecordsInfo(self._records)
 
     @property
-    def site_helper(self) -> SiteHelper:
+    def reports_info(self) -> ReportsInfo:
         """
-        SiteHelper used for interactions that do not require a UI
+        Navigate to reports and gather information about available reports
         """
-        return self._site_helper
+        return ReportsInfo(self._reports)
+
+    @property
+    def sites_info(self) -> SitesInfo:
+        """
+        Get Site metadata object
+        """
+        return SitesInfo(self._sites)
+
+    @property
+    def tasks_info(self) -> TasksInfo:
+        """
+        Navigate to tasks and gather information about available tasks
+        """
+        return TasksInfo(self._tasks)
+
+    @property
+    def visitor(self) -> Visitor:
+        """
+        Visitor that can be used to navigate to different types of pages in an Appian instance
+        """
+        return self._visitor
+
+    @property
+    def system_operator(self) -> SystemOperator:
+        """
+        Abstraction used for system operation that do not require a UI
+        """
+        return self._system_operator
 
     def login(self, auth: Optional[list] = None, check_login: bool = True) -> Tuple[HttpSession, Response]:
         return self._interactor.login(auth, check_login=check_login)
 
     def logout(self) -> None:
         """
         Logout from Appian
@@ -229,33 +274,36 @@
         super().__init__(parent)
 
         self.host = self.parent.host
 
         # A set of datatypes cached. Used to populate "X-Appian-Cached-Datatypes" header field
         self.cached_datatype: set = set()
 
-    def on_start(self, portals_mode: bool = False) -> None:
+    def on_start(self, portals_mode: bool = False, config_path: str = DEFAULT_CONFIG_PATH) -> None:
         """
         Overloaded function of Locust's default on_start.
 
         It will create object self.appian and logs in to Appian
 
         Args:
             portals_mode (bool): set to True if connecting to portals site
+            config_path (str): path to configuration file
         """
         self.portals_mode = portals_mode
         self.workerId = str(uuid.uuid4())
         base_path_override = self.parent.base_path_override \
             if hasattr(self.parent, "base_path_override") else ""
-        self._appian = AppianClient(self.client, self.host, base_path_override=base_path_override, portals_mode=portals_mode)
+        self._appian = AppianClient(self.client, self.host, base_path_override=base_path_override,
+                                    portals_mode=portals_mode, config_path=config_path)
         if not portals_mode:
             self.auth = self._determine_auth()
-            resp = self.appian.login(self.auth)
+            self.appian.login(self.auth)
+            resp = self.appian._interactor.get_page(uri=self.host + "/suite/tempo/news")
             test = r'\\\\\\/suite\\\\\\/rest\\\\\\/a\\\\\\/sites\\\\\\/latest\\\\\\/D6JMim\\\\\\/page\\\\\\/(.+)\\\\\\'
-            m = re.search(test, resp[1].text)
+            m = re.search(test, resp.text)
             if m is None or m.group(1) == 'news':
                 # old way
                 self.appian._interactor.url_pattern_version = 0
             elif m.group(1) == 'p.news':
                 # new way
                 self.appian._interactor.url_pattern_version = 1
             else:
@@ -359,7 +407,15 @@
     """
     Appian Locust SequentialTaskSet. Provides functionality of Locust's SequentialTaskSet and Handles creation of basic
     objects like``self.appian`` and actions like ``login`` and ``logout``
     """
 
     def __init__(self, parent: SequentialTaskSet) -> None:
         super(AppianTaskSequence, self).__init__(parent)
+
+
+class NoOpEvents():
+    def fire(self, *args: str, **kwargs: int) -> None:
+        pass
+
+    def context(self, *args: str, **kwargs: int) -> dict:
+        return {}
```

### Comparing `appian-locust-2.0.0a7/appian_locust/application_uiform.py` & `appian-locust-2.0.0a8/appian_locust/uiform/application_uiform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from typing import Any, Dict, Optional
 
-from ._design import _Design, get_available_design_objects
-from ._interactor import _Interactor
-from ._locust_error_handler import raises_locust_error
-from .design_object_uiform import DesignObjectUiForm
-from .design_object import DesignObject
-from .design_object_type import DesignObjectType
-from .helper import find_component_by_label_and_type_dict
-from .uiform import SailUiForm
+from .._design import _Design, get_available_design_objects
+from .._interactor import _Interactor
+from .._locust_error_handler import raises_locust_error
+from ..uiform import DesignObjectUiForm, SailUiForm
+from ..objects import DesignObject, DesignObjectType
+from ..utilities.helper import find_component_by_label_and_type_dict
 
 
 class ApplicationUiForm(SailUiForm):
 
     def __init__(self, interactor: _Interactor, state: Dict[str, Any], breadcrumb: str = "ApplicationUi"):
         super().__init__(interactor, state, breadcrumb)
         self.__design = _Design(interactor)
```

### Comparing `appian-locust-2.0.0a7/appian_locust/design_object_uiform.py` & `appian-locust-2.0.0a8/appian_locust/uiform/design_object_uiform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict
 
-from ._design import _Design
-from ._interactor import _Interactor
-from ._locust_error_handler import raises_locust_error
-from .uiform import SailUiForm
+from .._design import _Design
+from .._interactor import _Interactor
+from .._locust_error_handler import raises_locust_error
+from ..uiform import SailUiForm
 
 
 class DesignObjectUiForm(SailUiForm):
 
     def __init__(self, interactor: _Interactor, state: Dict[str, Any], breadcrumb: str = "DesignObjectUi"):
         super().__init__(interactor, state, breadcrumb)
         self.__design = _Design(interactor)
```

### Comparing `appian-locust-2.0.0a7/appian_locust/design_uiform.py` & `appian-locust-2.0.0a8/appian_locust/uiform/design_uiform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any, Dict, Optional
 
-from . import logger
-from ._design import _Design, get_available_design_objects
-from ._interactor import _Interactor
-from ._locust_error_handler import raises_locust_error
-from .application import Application
-from .application_uiform import ApplicationUiForm
-from .design_object import DesignObject
-from .helper import find_component_by_attribute_in_dict, find_component_by_label_and_type_dict
-from .uiform import SailUiForm
+from ..utilities import logger
+from .._design import _Design, get_available_design_objects
+from .._interactor import _Interactor
+from .._locust_error_handler import raises_locust_error
+from ..objects import Application, DesignObject
+from ..uiform import ApplicationUiForm, SailUiForm
+from ..objects import DesignObject
+from ..utilities.helper import find_component_by_attribute_in_dict, find_component_by_label_and_type_dict
 
 log = logger.getLogger(__name__)
 
 
 class DesignUiForm(SailUiForm):
 
     def __init__(self, interactor: _Interactor, state: Dict[str, Any], breadcrumb: str = "DesignUi"):
```

### Comparing `appian-locust-2.0.0a7/appian_locust/feature_flag.py` & `appian-locust-2.0.0a8/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a7/appian_locust/helper.py` & `appian-locust-2.0.0a8/appian_locust/utilities/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import random
 import re
 from typing import Any, Callable, Dict, Generator, List, Union, Optional
-from .exceptions import ComponentNotFoundException
+from ..exceptions import ComponentNotFoundException
 
 import gevent  # type: ignore
 from locust.env import Environment
 
 from . import logger
 
 ENV = Environment()
```

### Comparing `appian-locust-2.0.0a7/appian_locust/loadDriverUtils.py` & `appian-locust-2.0.0a8/appian_locust/utilities/loadDriverUtils.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,21 +17,22 @@
         "exec_start_end_task": 1,
     },
     "skip_machine_setup": False,
     "auth": ["username", "password"]
 }
 
 log = logger.getLogger(__name__)
+DEFAULT_CONFIG_PATH = "./config.json"
 
 
 class loadDriverUtils:
     def __init__(self) -> None:
         self.c = default_config
 
-    def load_config(self, config_file: str = "./config.json") -> dict:
+    def load_config(self, config_file: str = DEFAULT_CONFIG_PATH) -> dict:
         """
         Load a json configuration file into a dictionary
         Args:
             config_file: Location where config file can be found
 
         Returns (dict): Dictionary containing configuration. Will also be stored in
                         loadDriverUtils.c
@@ -41,13 +42,7 @@
             self.c = json.load(open(config_file))
             return self.c
         else:
             log.error("Failed to load config ({}), exiting.".format(config_file))
             log.error("Example config:{}".format(json.dumps(default_config,
                                                             indent=2)))
             exit(1)
-
-
-utils = loadDriverUtils()
-
-# Aliased for backwards compatability
-utls = utils
```

### Comparing `appian-locust-2.0.0a7/appian_locust/logger.py` & `appian-locust-2.0.0a8/appian_locust/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a7/appian_locust/news_info.py` & `appian-locust-2.0.0a8/appian_locust/info/news_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from requests.models import Response
 from typing import Any, Dict, Optional, Tuple
 
-from ._interactor import _Interactor
-from ._news import _News
+from .._interactor import _Interactor
+from .._news import _News
 
 
 class NewsInfo:
     """
     Class which provides metadata about news entries from the Tempo News tab
     """
 
@@ -26,15 +26,15 @@
 
         Examples:
 
             >>> news_info.get_all()
         """
         return self.__news.get_all(search_string=search_string, locust_request_label=locust_request_label)
 
-    def get_news(self, news_name: str, exact_match: bool = True, search_string: Optional[str] = None) -> Dict[str, Any]:
+    def get_news_entry(self, news_name: str, exact_match: bool = True, search_string: Optional[str] = None) -> Dict[str, Any]:
         """
         Get the information about specific news by name.
 
         Args:
             news_name (str): name of the news entry
             exact_match (bool, optional): Should news name match exactly or to be partial match. Default : True
             search_string (str, optional): results will be filtered based on the search string.
@@ -51,38 +51,14 @@
             If only partial name is known,
 
             >>> news_info.get_news("news_name", exact_match=False)
 
         """
         return self.__news.get_news(news_name, exact_match, search_string)
 
-    def visit_news_entry(self, news_name: str, exact_match: bool = True, search_string: Optional[str] = None) -> Tuple:
-        """
-        This function simulates navigating to a single entry in the ui. There are two parts to navigating to a
-        news entry: navigating to the view and getting the news entry's feed.
-
-        Args:
-            news_name (str): Name of the news entry to be called
-            exact_match (bool, optional): Should news name match exactly or to be partial match. Default : True
-            search_string (str, optional): results will be filtered based on the search string.
-
-        Returns (Tuple): Response codes for the view navigation and getting the feed entry
-
-        Examples:
-
-            If full name of news is known,
-
-            >>> news_info.visit_news_entry("news_name")
-
-            If only partial name is known,
-
-            >>> news_info.visit_news_entry("news_n", exact_match=False)
-        """
-        return self.__news.visit_news_entry(news_name, exact_match, search_string)
-
     def get_news_entry_related_records(self, news_name: str, exact_match: bool = True,
                                        search_string: Optional[str] = None,
                                        locust_request_label: Optional[str] = None) -> Optional[Response]:
         """
         Request related records information for a news entry
         Args:
             news_name (str): name of the news entry
```

### Comparing `appian-locust-2.0.0a7/appian_locust/record_list_uiform.py` & `appian-locust-2.0.0a8/appian_locust/uiform/record_list_uiform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, Optional
 from urllib.parse import quote
 
-from ._interactor import _Interactor
-from ._records_helper import get_all_records_from_json, get_records_from_json_by_column
+from .._interactor import _Interactor
+from .._records_helper import get_all_records_from_json, get_records_from_json_by_column
 from .uiform import SailUiForm
 
 
 class RecordListUiForm(SailUiForm):
     """
     UiForm representing a Record List from Tempo Records
     """
@@ -52,16 +52,15 @@
         response = self._interactor.get_page(uri=clear_uri, headers=headers, label=context_label)
         return RecordListUiForm(self._interactor, response.json(), breadcrumb=context_label)
 
     def get_visible_record_instances(self, column_index: Optional[int] = None) -> Dict[str, Any]:
         """
         Retrieve information about all visible records on the page.
         Args:
-            column_index: Which column to retrieve record information for. If no column is selected, every record link
-                          in the UI will be retrieved
+            column_index: Which column to retrieve record information for. If no column is selected, every record link in the UI will be retrieved.
 
         Returns: Dictionary with record instance information
         """
         if column_index is not None:
             record_instances, _ = get_records_from_json_by_column(self._state, column_index)
         else:
             record_instances, _ = get_all_records_from_json(self._state)
```

### Comparing `appian-locust-2.0.0a7/appian_locust/record_uiform.py` & `appian-locust-2.0.0a8/appian_locust/uiform/record_uiform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict
 
-from ._interactor import _Interactor
-from ._records_helper import get_record_header_response, get_record_summary_view_response
+from .._interactor import _Interactor
+from .._records_helper import get_record_header_response, get_record_summary_view_response
 from .uiform import SailUiForm
 
 
 class RecordInstanceUiForm(SailUiForm):
     """
     UiForm representing a Record Instance UI. Supports both summary and header record views. Defaults to summary view
     """
```

### Comparing `appian-locust-2.0.0a7/appian_locust/records_info.py` & `appian-locust-2.0.0a8/appian_locust/info/records_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict
 
-from ._locust_error_handler import log_locust_error
-from ._records import _Records
+from .._locust_error_handler import log_locust_error
+from .._records import _Records
 
 
 class RecordsInfo():
     """
     Class which provides metadata about available record types from the Tempo Records tab
     """
```

### Comparing `appian-locust-2.0.0a7/appian_locust/reports_info.py` & `appian-locust-2.0.0a8/appian_locust/info/reports_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional
 
-from ._reports import _Reports
+from .._reports import _Reports
 
 
 class ReportsInfo:
     """
     Class which provides metadata about available reports from the Tempo Reports tab
     """
```

### Comparing `appian-locust-2.0.0a7/appian_locust/site_helper.py` & `appian-locust-2.0.0a8/appian_locust/system_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from requests.models import Response
 from typing import Optional, Dict, Any
 
 from ._actions import _Actions
 from ._interactor import _Interactor
 
 
-class SiteHelper:
+class SystemOperator:
     """
     Class for providing the ability to perform activities that do not require a UI interaction
-    to perform. For example, triggering an action without a startform.
+    i.e. triggering an action without a startform.
     """
 
     def __init__(self, interactor: _Interactor, actions: _Actions):
         self.__interactor = interactor
         self.__actions = actions
 
     def start_action(self, action_name: str, skip_design_call: bool = False,
```

### Comparing `appian-locust-2.0.0a7/appian_locust/sites_info.py` & `appian-locust-2.0.0a8/appian_locust/info/sites_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 
-from ._sites import _Sites
-from .site_objects import Site
+from .._sites import _Sites
+from ..objects import Site
 
 
 class SitesInfo:
     """
     Class which provides metadata about available Sites
     """
```

### Comparing `appian-locust-2.0.0a7/appian_locust/tasks_info.py` & `appian-locust-2.0.0a8/appian_locust/info/tasks_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict
 
-from ._tasks import _Tasks
+from .._tasks import _Tasks
 
 
 class TasksInfo:
     """
     Class which provides metadata about available tasks from the Tempo Tasks tab
     """
```

### Comparing `appian-locust-2.0.0a7/appian_locust/uiform.py` & `appian-locust-2.0.0a8/appian_locust/uiform/uiform.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,45 +5,38 @@
 import os
 import random
 import warnings
 from typing import Any, Dict, List, Union, Optional, TYPE_CHECKING
 from urllib.parse import quote, urlparse
 from copy import deepcopy
 
-from appian_locust._records_helper import _is_grid
-
-from . import logger
-from ._grid_interactor import GridInteractor
-from ._interactor import _Interactor
-from ._locust_error_handler import raises_locust_error
-from ._task_opener import _TaskOpener
-from ._ui_reconciler import UiReconciler
-from .exceptions import InvalidComponentException, ChoiceNotFoundException
-from .helper import (extract_all_by_label, find_component_by_attribute_and_index_in_dict,
+from ..utilities import logger
+from .._grid_interactor import GridInteractor
+from .._interactor import _Interactor
+from .._locust_error_handler import raises_locust_error
+from .._task_opener import _TaskOpener
+from .._ui_reconciler import UiReconciler
+from ..exceptions import InvalidComponentException, ChoiceNotFoundException
+from ..utilities.helper import (extract_all_by_label, find_component_by_attribute_and_index_in_dict,
                      find_component_by_attribute_in_dict, find_component_by_index_in_dict,
                      find_component_by_label_and_type_dict, find_component_by_type_and_attribute_and_index_in_dict)
-from ._records_helper import (get_url_stub_from_record_list_url_path)
+from .._records_helper import get_url_stub_from_record_list_url_path, _is_grid
 
 if TYPE_CHECKING:
-    from .record_uiform import RecordInstanceUiForm
+    from ..uiform import RecordInstanceUiForm
 
 KEY_UUID = "uuid"
 KEY_CONTEXT = "context"
 START_PROCESS_LINK_TYPE = 'StartProcessLink'
 PROCESS_TASK_LINK_TYPE = 'ProcessTaskLink'
 COMPONENTS_THAT_CAN_BE_FILLED = ["ParagraphField", "TextField", "SearchBoxWidget"]
 
 log = logger.getLogger(__name__)
 
 
-class ClientMode(enum.Enum):
-    TEMPO = 'TEMPO'
-    DESIGN = 'DESIGN'
-
-
 class SailUiForm:
     def __init__(self, interactor: _Interactor, state: Dict[str, Any], breadcrumb: str = "SailUi"):
         """
         Appian rendered UI that provides page interactivity. ``SailUiForm`` is a base class that is abstracted
         by specific Appian form types to handle requirements or provide metadata unique to that page.
 
         Args:
```

### Comparing `appian-locust-2.0.0a7/appian_locust/visitor.py` & `appian-locust-2.0.0a8/appian_locust/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from typing import Optional
 
-from appian_locust.record_uiform import RecordInstanceUiForm
-from ._portals import _Portals
-from .application_uiform import ApplicationUiForm
-from .design_object_uiform import DesignObjectUiForm
-from .design_uiform import DesignUiForm
-from .design_object_type import DesignObjectType
-from .record_list_uiform import RecordListUiForm
-from .site_objects import PageType
-from .uiform import SailUiForm
 from ._actions import _Actions
 from ._design import _Design
 from ._interactor import _Interactor
+from ._portals import _Portals
 from ._records import _Records
 from ._reports import _Reports
 from ._sites import _Sites
 from ._admin import _Admin
 from ._tasks import _Tasks
-from .helper import format_label
+from .utilities.helper import format_label
+from .objects import DesignObjectType, PageType
+from .uiform import ApplicationUiForm, DesignUiForm, DesignObjectUiForm, RecordInstanceUiForm, RecordListUiForm, SailUiForm
 
 
 class Visitor:
     """
     Provides methods to get an interactable ``SailUiForm`` from an Appian instance. Each method will return the respected ``SailUiForm`` type for which it will allow
     interactions with the visited page.
     """
@@ -182,15 +176,15 @@
         """
         self.__records.get_records_nav(locust_request_label=locust_request_label)
         form_json = self.__records.visit_record_type(record_type, exact_match=exact_match, is_mobile=is_mobile,
                                                      locust_request_label=locust_request_label)
         breadcrumb = f'Records.{record_type}.RecordListUi'
         return RecordListUiForm(self.__interactor, form_json, breadcrumb=breadcrumb)
 
-    def visit_site(self, site_name: str, page_name: str) -> 'SailUiForm':
+    def visit_site(self, site_name: str, page_name: str) -> SailUiForm:
         """
         Get a SailUiForm for a Task, Report or Action
 
         Args:
             site_name(str): Site where the page exists
             page_name(str): Page to navigate to
```

### Comparing `appian-locust-2.0.0a7/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.0.0a8/appian_locust.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a7
+Version: 2.0.0a8
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -75,15 +75,15 @@
     [pipenv]
     allow_prereleases = true
 
 2. Configure your test to point at the Appian instance you will be using.
 You can use example file provided in this repository `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_:
 
 - Set ``host_address`` to the address of your Appian instance.
-- In ``auth``, specify the username and password of the user account to use.
+- In ``auth``, specify the username and password of the user account to use. Note: This user must be able to access Tempo.
 
 .. code-block:: json
 
     {
         "host_address": "site-name.appiancloud.com",
         "auth": [
             "user.name",
```

### Comparing `appian-locust-2.0.0a7/setup.cfg` & `appian-locust-2.0.0a8/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a7/setup.py` & `appian-locust-2.0.0a8/setup.py`

 * *Files identical despite different names*

