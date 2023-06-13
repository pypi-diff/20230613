# Comparing `tmp/anycluster-2.3.1.tar.gz` & `tmp/anycluster-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.3.1.tar", last modified: Mon Jun 12 05:58:22 2023, max compression
+gzip compressed data, was "anycluster-2.3.2.tar", last modified: Tue Jun 13 06:43:49 2023, max compression
```

## Comparing `anycluster-2.3.1.tar` & `anycluster-2.3.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.963686 anycluster-2.3.1/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.1/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.1/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-12 05:58:22.963686 anycluster-2.3.1/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.1/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.1/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3656 2023-05-26 12:34:24.000000 anycluster-2.3.1/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    37218 2023-06-07 12:40:46.000000 anycluster-2.3.1/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.1/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.1/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.1/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.1/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3918 2023-06-06 10:47:45.000000 anycluster-2.3.1/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.1/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     7902 2023-06-07 12:40:00.000000 anycluster-2.3.1/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.1/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3670 2023-06-06 10:10:33.000000 anycluster-2.3.1/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.1/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.3.1/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.1/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.3.1/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.1/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.1/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9915 2023-06-12 05:58:07.000000 anycluster-2.3.1/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.1/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.1/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.963686 anycluster-2.3.1/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.963686 anycluster-2.3.1/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.963686 anycluster-2.3.1/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.1/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.1/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.1/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.1/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.1/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    14813 2023-05-26 08:50:17.000000 anycluster-2.3.1/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.1/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.1/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.1/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.1/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    25353 2023-05-26 08:50:15.000000 anycluster-2.3.1/anycluster/tests/test_MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.1/anycluster/utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-12 05:58:22.963686 anycluster-2.3.1/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-12 05:56:19.000000 anycluster-2.3.1/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.706701 anycluster-2.3.2/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.2/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.2/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-13 06:43:49.706701 anycluster-2.3.2/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.2/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.698701 anycluster-2.3.2/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.2/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3536 2023-06-13 06:05:24.000000 anycluster-2.3.2/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    38198 2023-06-13 05:56:27.000000 anycluster-2.3.2/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.2/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.2/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.2/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.2/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     4685 2023-06-13 06:41:38.000000 anycluster-2.3.2/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.2/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     8087 2023-06-12 13:31:27.000000 anycluster-2.3.2/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.2/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5293 2023-06-13 06:41:37.000000 anycluster-2.3.2/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.2/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2829 2023-06-13 06:32:28.000000 anycluster-2.3.2/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.2/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3519 2023-06-13 06:32:18.000000 anycluster-2.3.2/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.2/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.2/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10055 2023-06-12 13:28:29.000000 anycluster-2.3.2/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.2/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.2/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.698701 anycluster-2.3.2/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.698701 anycluster-2.3.2/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.706701 anycluster-2.3.2/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.706701 anycluster-2.3.2/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.2/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.2/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.2/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.2/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.2/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    16331 2023-06-12 12:46:45.000000 anycluster-2.3.2/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.2/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.2/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.2/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.2/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    27459 2023-06-12 12:46:42.000000 anycluster-2.3.2/anycluster/tests/test_MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.2/anycluster/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-13 06:43:49.706701 anycluster-2.3.2/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-13 06:43:29.000000 anycluster-2.3.2/setup.py
```

### Comparing `anycluster-2.3.1/LICENSE` & `anycluster-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/PKG-INFO` & `anycluster-2.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.3.1
+Version: 2.3.2
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.3.1/README.md` & `anycluster-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/ClusterCache.py` & `anycluster-2.3.2/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/FilterComposer.py` & `anycluster-2.3.2/anycluster/FilterComposer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,29 @@
         filters = [
             {"column": db_column_name, "values": value, "operator": operator_string }
         ]
     
 ------------------------------------------------------------------------------------------------------------------------'''
 import numbers, decimal
 
-# IMPLEMENT: check settings.ANYVLUSTER_ALLOWED_FILTER_COLUMNS
-class FilterComposer:
+OPERATOR_MAPPING = {
+    '=': '=',
+    '!=': '!=',
+    '>=': '>=',
+    '<=': '<=',
+    'startswith': '~',
+    'contains': '~'
+}
+
+LIST_OPERATOR_MAPPING = {
+    'in': 'IN',
+    'not in': 'NOT IN',
+}
 
-    operator_mapping = {
-        '=': '=',
-        '!=': '!=',
-        '>=': '>=',
-        '<=': '<=',
-        'startswith': '~',
-        'contains': '~'
-    }
-
-    list_operator_mapping = {
-        'in': 'IN',
-        'not in': 'NOT IN',
-    }
+class FilterComposer:
     
     def __init__(self, filters):
         self.filters = filters
 
     def parse_filter_value(self, operator, value):
 
         if type(value) == str:
@@ -67,23 +66,23 @@
         column = filter['column']
         comparison_operator = filter['operator']
         value = filter['value']
 
         filterstring += '('
 
         if isinstance(value, list):
-            parsed_operator = self.list_operator_mapping[comparison_operator]
+            parsed_operator = LIST_OPERATOR_MAPPING[comparison_operator]
 
             sql_value = str(tuple(value))
 
             filterstring += '{column} {operator} {sql_value}'.format(column=column, operator=parsed_operator,
                                                                     sql_value=sql_value)
 
         else:
-            parsed_operator = self.operator_mapping[comparison_operator]
+            parsed_operator = OPERATOR_MAPPING[comparison_operator]
 
             sql_value = self.parse_filter_value(comparison_operator, value)
 
             filterstring += '{column} {operator} {sql_value}'.format(column=column, operator=parsed_operator,
                                                                     sql_value=sql_value)
 
         filterstring += ')'
```

### Comparing `anycluster-2.3.1/anycluster/MapClusterer.py` & `anycluster-2.3.2/anycluster/MapClusterer.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,17 +115,14 @@
         self.schema_name = schema_name
 
         # the srid of the database, falls back to 4326
         self.db_srid = self.get_database_srid()
 
         self.maptools = MapTools(int(maptile_size))
 
-        # filter operators
-        self.valid_operators = ['=', '<', '>', '<=', '>=', 'list', '!list']
-
     # read the srid of the database.
 
     def get_database_srid(self):
 
         db_srid = None
 
         srid_qry = 'SELECT id, ST_SRID({geo_column}) FROM {schema_name}.{geo_table} LIMIT 1;'.format(
@@ -515,16 +512,15 @@
                     ) AS ksub
 
                     GROUP BY id
                     ORDER BY kmeans;
                     
                 '''.format(geo_column=geo_column_str, pin_qry_0=pin_qry[0], pin_qry_1=pin_qry[1], k=k,
                            schema_name=self.schema_name, geo_table=geo_table, geos_geometry=geos_geometry.ewkt,
-                           filterstring=filterstring, additional_column_qry_0=additional_column_qry[
-                               0],
+                           filterstring=filterstring, additional_column_qry_0=additional_column_qry[0],
                            additional_column_qry_1=additional_column_qry[1])
 
                 with connections['default'].cursor() as cursor:
                     cursor.execute(sql)
 
                     cluster_rows = cursor.fetchall()
 
@@ -834,52 +830,76 @@
         query_result = cursor.fetchone()
 
         count += query_result[0]
 
         return count
 
 
+    def get_additional_group_by_columns_string(self):
+
+        column_names = getattr(settings, 'ANYCLUSTER_ADDITIONAL_GROUP_BY_COLUMNS', [])
+
+        additional_group_by_columns_string = ''
+
+        for column_name in column_names:
+            additional_group_by_columns_string = '{additional_group_by_columns_string}, MIN({column}::VARCHAR) AS {column}'.format(
+                additional_group_by_columns_string=additional_group_by_columns_string, column=column_name)
+
+        return additional_group_by_columns_string
+
+
     def get_grouped_map_contents(self, geojson, geometry_type, zoom, filters, group_by):
 
         # currently, the geometry type for counting is always set to GEOMETRY_TYPE_AREA,
         # because otherwise pins which are outside the current viewport, but inside the cluster geometry would be counted
         # the pins visible on the map would not always be the returned count if GEOMETRY_TYPE_VIEWPORT was supported
         geometry_type = GEOMETRY_TYPE_AREA
 
         geometries_for_counting = self.get_geometries_for_counting(geojson, geometry_type, zoom)
 
         geom_filterstring = self.get_geom_filter_string_from_geos(geometries_for_counting)
         
         filter_composer = FilterComposer(filters)
         filterstring = filter_composer.as_sql()
 
+        additional_group_by_columns_string = self.get_additional_group_by_columns_string()
+
         groups = {}
 
         grouped_count_sql = '''
-            SELECT COUNT(id), {group_by}
+            SELECT COUNT(id), {group_by} {additional_group_by_columns_string}
             FROM {schema_name}.{geo_table}
                 WHERE {geo_column_str} IS NOT NULL
                     AND {geom_filterstring} {filterstring}
                         GROUP BY {group_by} ORDER BY {group_by} ASC;
         '''.format(schema_name=self.schema_name, geo_table=geo_table, geo_column_str=geo_column_str,
-                    geom_filterstring=geom_filterstring, filterstring=filterstring, group_by=group_by)
+                    geom_filterstring=geom_filterstring, filterstring=filterstring, group_by=group_by,
+                    additional_group_by_columns_string=additional_group_by_columns_string)
 
         cursor = connections['default'].cursor()
         cursor.execute(grouped_count_sql)
         results = cursor.fetchall()
+
+        additional_column_names = getattr(settings, 'ANYCLUSTER_ADDITIONAL_GROUP_BY_COLUMNS', [])
         
         for result in results:
             count = result[0]
             group_name = str(result[1])
 
             if group_name not in groups:
                 groups[group_name] = {
                     'count' : count,
                 }
 
+                #groups[group_name][group_by] = group_name
+
+                for index, additional_column in enumerate(additional_column_names, 0):
+                    query_index = index + 2
+                    groups[group_name][additional_column] = result[query_index]
+
             else:
                 groups[group_name]['count'] += count
         
         return groups
 
 
     '''---------------------------------------------------------------------------------------------------------------------
```

### Comparing `anycluster-2.3.1/anycluster/MapTools.py` & `anycluster-2.3.2/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/__pycache__/json_schemas.cpython-38.pyc` & `anycluster-2.3.2/anycluster/api/__pycache__/json_schemas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc` & `anycluster-2.3.2/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/__pycache__/urls.cpython-38.pyc` & `anycluster-2.3.2/anycluster/api/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/__pycache__/views.cpython-38.pyc` & `anycluster-2.3.2/anycluster/api/__pycache__/views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun  7 12:39:54 2023 UTC, .py size: 9942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9a7a 8064 d626 0000  U........z.d.&..
+00000000: 550d 0d0a 0000 0000 7d1d 8764 4727 0000  U.......}..dG'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6001 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -421,74 +421,86 @@
 00001a40: 0801 0a02 0e01 02ff 0201 02ff 0403 1202  ................
 00001a50: 0e02 7a17 4765 744d 6170 436f 6e74 656e  ..z.GetMapConten
 00001a60: 7443 6f75 6e74 2e70 6f73 744e 725d 0000  tCount.postNr]..
 00001a70: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
 00001a80: 7220 0000 0072 6a00 0000 ec00 0000 7302  r ...rj.......s.
 00001a90: 0000 0008 0272 6a00 0000 6300 0000 0000  .....rj...c.....
 00001aa0: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00001ab0: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00001ac0: 6401 6402 8400 5a03 6403 5300 2904 da15  d.d...Z.d.S.)...
-00001ad0: 4765 7447 726f 7570 6564 4d61 7043 6f6e  GetGroupedMapCon
-00001ae0: 7465 6e74 7363 0200 0000 0000 0000 0000  tentsc..........
-00001af0: 0000 0e00 0000 0700 0000 4f00 0000 73a8  ..........O...s.
-00001b00: 0000 0074 007c 016a 0164 018d 017d 047c  ...t.|.j.d...}.|
-00001b10: 04a0 02a1 0072 9864 027d 057c 046a 0364  .....r.d.}.|.j.d
-00001b20: 0319 007d 067c 046a 0364 0419 007d 077c  ...}.|.j.d...}.|
-00001b30: 00a0 047c 046a 0364 0519 00a1 017d 087c  ...|.j.d.....}.|
-00001b40: 046a 0364 0619 007d 097c 0364 0719 007d  .j.d...}.|.d...}
-00001b50: 0a7c 046a 0364 0819 007d 0b7c 006a 057c  .|.j.d...}.|.j.|
-00001b60: 0774 067c 067c 057c 087c 0166 067c 038e  .t.|.|.|.|.f.|..
-00001b70: 017d 0c7c 0ca0 077c 097c 077c 0a7c 067c  .}.|...|.|.|.|.|
-00001b80: 0ba1 057d 0d74 087c 0d83 0101 0074 097c  ...}.t.|.....t.|
-00001b90: 0d74 0a6a 0b64 098d 0253 0074 097c 046a  .t.j.d...S.t.|.j
-00001ba0: 0c74 0a6a 0d64 098d 0253 0029 0a4e 724f  .t.j.d...S.).NrO
-00001bb0: 0000 0054 7236 0000 0072 3400 0000 722c  ...Tr6...r4...r,
-00001bc0: 0000 0072 5000 0000 7231 0000 00da 0867  ...rP...r1.....g
-00001bd0: 726f 7570 5f62 7972 0800 0000 290e 7214  roup_byr....).r.
-00001be0: 0000 0072 4a00 0000 7251 0000 0072 5200  ...rJ...rQ...rR.
-00001bf0: 0000 722d 0000 0072 3900 0000 720f 0000  ..r-...r9...r...
-00001c00: 005a 1867 6574 5f67 726f 7570 6564 5f6d  .Z.get_grouped_m
-00001c10: 6170 5f63 6f6e 7465 6e74 73da 0570 7269  ap_contents..pri
-00001c20: 6e74 7206 0000 0072 0900 0000 7253 0000  ntr....r....rS..
-00001c30: 0072 5400 0000 7255 0000 0029 0e72 1b00  .rT...rU...).r..
-00001c40: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00001c50: 0072 4c00 0000 7237 0000 0072 3600 0000  .rL...r7...r6...
-00001c60: 7234 0000 0072 2c00 0000 7250 0000 0072  r4...r,...rP...r
-00001c70: 3100 0000 726d 0000 0072 4b00 0000 da06  1...rm...rK.....
-00001c80: 6772 6f75 7073 721f 0000 0072 1f00 0000  groupsr....r....
-00001c90: 7220 0000 0072 5700 0000 0901 0000 7324  r ...rW.......s$
-00001ca0: 0000 0000 020c 0208 0204 010a 010a 0110  ................
-00001cb0: 020a 0108 020a 020e 0102 ff02 0102 ff04  ................
-00001cc0: 0312 0208 020e 027a 1a47 6574 4772 6f75  .......z.GetGrou
-00001cd0: 7065 644d 6170 436f 6e74 656e 7473 2e70  pedMapContents.p
-00001ce0: 6f73 744e 725d 0000 0072 1f00 0000 721f  ostNr]...r....r.
-00001cf0: 0000 0072 1f00 0000 7220 0000 0072 6c00  ...r....r ...rl.
-00001d00: 0000 0701 0000 7302 0000 0008 0272 6c00  ......s......rl.
-00001d10: 0000 292a da0b 646a 616e 676f 2e63 6f6e  ..)*..django.con
-00001d20: 6672 0200 0000 da0b 646a 616e 676f 2e63  fr......django.c
-00001d30: 6f72 6572 0300 0000 da14 7265 7374 5f66  orer......rest_f
-00001d40: 7261 6d65 776f 726b 2e76 6965 7773 7204  ramework.viewsr.
-00001d50: 0000 00da 1772 6573 745f 6672 616d 6577  .....rest_framew
-00001d60: 6f72 6b2e 7265 7370 6f6e 7365 7206 0000  ork.responser...
-00001d70: 00da 1872 6573 745f 6672 616d 6577 6f72  ...rest_framewor
-00001d80: 6b2e 7265 6e64 6572 6572 7372 0700 0000  k.renderersr....
-00001d90: da0e 7265 7374 5f66 7261 6d65 776f 726b  ..rest_framework
-00001da0: 7209 0000 005a 1761 6e79 636c 7573 7465  r....Z.anycluste
-00001db0: 722e 4d61 7043 6c75 7374 6572 6572 720a  r.MapClustererr.
-00001dc0: 0000 0072 0b00 0000 da16 616e 7963 6c75  ...r......anyclu
-00001dd0: 7374 6572 2e64 6566 696e 6974 696f 6e73  ster.definitions
-00001de0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00001df0: 0f00 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
-00001e00: 0000 0072 1400 0000 7215 0000 00da 0a61  ...r....r......a
-00001e10: 6e79 636c 7573 7465 7272 1600 0000 5a10  nyclusterr....Z.
-00001e20: 616e 7963 6c75 7374 6572 2e75 7469 6c73  anycluster.utils
-00001e30: 7217 0000 00da 0767 6574 6174 7472 5a13  r......getattrZ.
-00001e40: 6769 735f 7365 7269 616c 697a 6572 5f70  gis_serializer_p
-00001e50: 6174 6872 4900 0000 da04 6a73 6f6e 7219  athrI.....jsonr.
-00001e60: 0000 0072 2600 0000 724e 0000 0072 5b00  ...r&...rN...r[.
-00001e70: 0000 725e 0000 0072 6300 0000 7266 0000  ..r^...rc...rf..
-00001e80: 0072 6a00 0000 726c 0000 0072 1f00 0000  .rj...rl...r....
-00001e90: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-00001ea0: 083c 6d6f 6475 6c65 3e01 0000 0073 2c00  .<module>....s,.
-00001eb0: 0000 0c01 0c02 0c01 0c01 0c01 0c02 1001  ................
-00001ec0: 1802 1c03 0c01 0c02 0c01 0802 0802 1006  ................
-00001ed0: 0e38 1220 121e 1225 121f 1215 121b       .8. ...%......
+00001ab0: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00001ac0: 6401 6402 8400 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
+00001ad0: 6405 5300 2906 da15 4765 7447 726f 7570  d.S.)...GetGroup
+00001ae0: 6564 4d61 7043 6f6e 7465 6e74 7363 0200  edMapContentsc..
+00001af0: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+00001b00: 0000 4300 0000 7304 0000 007c 0153 0072  ..C...s....|.S.r
+00001b10: 3a00 0000 721f 0000 0029 0272 1b00 0000  :...r....).r....
+00001b20: da06 6772 6f75 7073 721f 0000 0072 1f00  ..groupsr....r..
+00001b30: 0000 7220 0000 00da 0e70 7265 7061 7265  ..r .....prepare
+00001b40: 5f67 726f 7570 730a 0100 0073 0200 0000  _groups....s....
+00001b50: 0001 7a24 4765 7447 726f 7570 6564 4d61  ..z$GetGroupedMa
+00001b60: 7043 6f6e 7465 6e74 732e 7072 6570 6172  pContents.prepar
+00001b70: 655f 6772 6f75 7073 6302 0000 0000 0000  e_groupsc.......
+00001b80: 0000 0000 000f 0000 0007 0000 004f 0000  .............O..
+00001b90: 0073 aa00 0000 7400 7c01 6a01 6401 8d01  .s....t.|.j.d...
+00001ba0: 7d04 7c04 a002 a100 729a 6402 7d05 7c04  }.|.....r.d.}.|.
+00001bb0: 6a03 6403 1900 7d06 7c04 6a03 6404 1900  j.d...}.|.j.d...
+00001bc0: 7d07 7c00 a004 7c04 6a03 6405 1900 a101  }.|...|.j.d.....
+00001bd0: 7d08 7c04 6a03 6406 1900 7d09 7c03 6407  }.|.j.d...}.|.d.
+00001be0: 1900 7d0a 7c04 6a03 6408 1900 7d0b 7c00  ..}.|.j.d...}.|.
+00001bf0: 6a05 7c07 7406 7c06 7c05 7c08 7c01 6606  j.|.t.|.|.|.|.f.
+00001c00: 7c03 8e01 7d0c 7c0c a007 7c09 7c07 7c0a  |...}.|...|.|.|.
+00001c10: 7c06 7c0b a105 7d0d 7c00 a008 7c0d a101  |.|...}.|...|...
+00001c20: 7d0e 7409 7c0e 740a 6a0b 6409 8d02 5300  }.t.|.t.j.d...S.
+00001c30: 7409 7c04 6a0c 740a 6a0d 6409 8d02 5300  t.|.j.t.j.d...S.
+00001c40: 290a 4e72 4f00 0000 5472 3600 0000 7234  ).NrO...Tr6...r4
+00001c50: 0000 0072 2c00 0000 7250 0000 0072 3100  ...r,...rP...r1.
+00001c60: 0000 da08 6772 6f75 705f 6279 7208 0000  ....group_byr...
+00001c70: 0029 0e72 1400 0000 724a 0000 0072 5100  .).r....rJ...rQ.
+00001c80: 0000 7252 0000 0072 2d00 0000 7239 0000  ..rR...r-...r9..
+00001c90: 0072 0f00 0000 5a18 6765 745f 6772 6f75  .r....Z.get_grou
+00001ca0: 7065 645f 6d61 705f 636f 6e74 656e 7473  ped_map_contents
+00001cb0: 726e 0000 0072 0600 0000 7209 0000 0072  rn...r....r....r
+00001cc0: 5300 0000 7254 0000 0072 5500 0000 290f  S...rT...rU...).
+00001cd0: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00001ce0: 1e00 0000 724c 0000 0072 3700 0000 7236  ....rL...r7...r6
+00001cf0: 0000 0072 3400 0000 722c 0000 0072 5000  ...r4...r,...rP.
+00001d00: 0000 7231 0000 0072 6f00 0000 724b 0000  ..r1...ro...rK..
+00001d10: 0072 6d00 0000 da0f 7072 6570 6172 6564  .rm.....prepared
+00001d20: 5f67 726f 7570 7372 1f00 0000 721f 0000  _groupsr....r...
+00001d30: 0072 2000 0000 7257 0000 000d 0100 0073  .r ...rW.......s
+00001d40: 2400 0000 0002 0c02 0802 0401 0a01 0a01  $...............
+00001d50: 1002 0a01 0802 0a02 0e01 02ff 0201 02ff  ................
+00001d60: 0403 1202 0a02 0e02 7a1a 4765 7447 726f  ........z.GetGro
+00001d70: 7570 6564 4d61 7043 6f6e 7465 6e74 732e  upedMapContents.
+00001d80: 706f 7374 4e29 0572 2300 0000 7224 0000  postN).r#...r$..
+00001d90: 0072 2500 0000 726e 0000 0072 5700 0000  .r%...rn...rW...
+00001da0: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00001db0: 2000 0000 726c 0000 0007 0100 0073 0400   ...rl.......s..
+00001dc0: 0000 0803 0803 726c 0000 0029 2ada 0b64  ......rl...)*..d
+00001dd0: 6a61 6e67 6f2e 636f 6e66 7202 0000 00da  jango.confr.....
+00001de0: 0b64 6a61 6e67 6f2e 636f 7265 7203 0000  .django.corer...
+00001df0: 00da 1472 6573 745f 6672 616d 6577 6f72  ...rest_framewor
+00001e00: 6b2e 7669 6577 7372 0400 0000 da17 7265  k.viewsr......re
+00001e10: 7374 5f66 7261 6d65 776f 726b 2e72 6573  st_framework.res
+00001e20: 706f 6e73 6572 0600 0000 da18 7265 7374  ponser......rest
+00001e30: 5f66 7261 6d65 776f 726b 2e72 656e 6465  _framework.rende
+00001e40: 7265 7273 7207 0000 00da 0e72 6573 745f  rersr......rest_
+00001e50: 6672 616d 6577 6f72 6b72 0900 0000 5a17  frameworkr....Z.
+00001e60: 616e 7963 6c75 7374 6572 2e4d 6170 436c  anycluster.MapCl
+00001e70: 7573 7465 7265 7272 0a00 0000 720b 0000  ustererr....r...
+00001e80: 00da 1661 6e79 636c 7573 7465 722e 6465  ...anycluster.de
+00001e90: 6669 6e69 7469 6f6e 7372 0c00 0000 720d  finitionsr....r.
+00001ea0: 0000 0072 0e00 0000 720f 0000 0072 1100  ...r....r....r..
+00001eb0: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00001ec0: 0072 1500 0000 da0a 616e 7963 6c75 7374  .r......anyclust
+00001ed0: 6572 7216 0000 005a 1061 6e79 636c 7573  err....Z.anyclus
+00001ee0: 7465 722e 7574 696c 7372 1700 0000 da07  ter.utilsr......
+00001ef0: 6765 7461 7474 725a 1367 6973 5f73 6572  getattrZ.gis_ser
+00001f00: 6961 6c69 7a65 725f 7061 7468 7249 0000  ializer_pathrI..
+00001f10: 00da 046a 736f 6e72 1900 0000 7226 0000  ...jsonr....r&..
+00001f20: 0072 4e00 0000 725b 0000 0072 5e00 0000  .rN...r[...r^...
+00001f30: 7263 0000 0072 6600 0000 726a 0000 0072  rc...rf...rj...r
+00001f40: 6c00 0000 721f 0000 0072 1f00 0000 721f  l...r....r....r.
+00001f50: 0000 0072 2000 0000 da08 3c6d 6f64 756c  ...r .....<modul
+00001f60: 653e 0100 0000 732c 0000 000c 010c 020c  e>....s,........
+00001f70: 010c 010c 010c 0210 0118 021c 030c 010c  ................
+00001f80: 020c 0108 0208 0210 060e 3812 2012 1e12  ..........8. ...
+00001f90: 2512 1f12 1512 1b                        %......
```

### Comparing `anycluster-2.3.1/anycluster/api/json_schemas.py` & `anycluster-2.3.2/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/serializers.py` & `anycluster-2.3.2/anycluster/api/serializers.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,29 +4,57 @@
 import jsonschema
 
 from .json_schemas import FEATURE_OR_FEATURECOLLECTION_SCHEMA
 
 from anycluster.definitions import GEOMETRY_TYPES, GEOMETRY_TYPE_VIEWPORT
 from anycluster.MapClusterer import Gis
 
+from anycluster.FilterComposer import OPERATOR_MAPPING, LIST_OPERATOR_MAPPING
+
+VALID_OPERATORS = list(OPERATOR_MAPPING.keys())
+VALID_LIST_OPERATORS = list(LIST_OPERATOR_MAPPING.keys())
 
 def filters_are_allowed(filters):
 
     for filter in filters:
 
         is_nested = 'filters' in filter
 
         if is_nested == False:
             column = filter.get('column', None)
+
+            operator = filter.get('operator', None)
+
+            value = filter.get('value', None)
+
             if not column:
-                raise serializers.ValidationError('Filter require a column')
+                raise serializers.ValidationError('Filters require a column')
         
             if column not in settings.ANYCLUSTER_FILTERS:
                 raise serializers.ValidationError('It is not allowed to filter Column {0}'.format(column))
-        
+
+            if value == None:
+                raise serializers.ValidationError('Filters require a value')
+
+            if not operator:
+                raise serializers.ValidationError('Filters require an operator')
+            
+            if isinstance(value, list):
+                if operator not in VALID_LIST_OPERATORS:
+                    message = 'Invalid operator: {0}. Allowed list operators are: {1}'.format(operator,
+                        ','.join(VALID_LIST_OPERATORS))
+                    raise serializers.ValidationError(message)
+            
+            else:
+                if operator not in VALID_OPERATORS:
+                    message = 'Invalid operator: {0}. Allowed operators are: {1}'.format(operator,
+                        ','.join(VALID_OPERATORS))
+                    raise serializers.ValidationError(message)
+
+            
         else:
             filters_are_allowed(filter['filters'])
 
 # needs to supprt FeatureCollection and Multipolygon
 class ClusterRequestSerializer(serializers.Serializer):
 
     output_srid = serializers.CharField(default='EPSG:4326', required=False, write_only=True)
@@ -73,16 +101,27 @@
     # additional filters, which are applied on top of filters, only for the count query
     modulations = serializers.JSONField(required=False, default={}, write_only=True)
 
     def validate_modulations(self, value):
 
         if value:
 
+            if not isinstance(value, dict):
+                raise serializers.ValidationError('Modulations have to be of type dict')
+
+            # modulation can be a filter or a nested filter
             for modulation_name, modulation in value.items():
-                filters_are_allowed(modulation['filters'])
+
+                if not isinstance(modulation_name, str):
+                    raise serializers.ValidationError('Invalid modulation key: {0}'.format(modulation_name))
+
+                if not isinstance(modulation, dict):
+                    raise serializers.ValidationError('Invalid modulation')
+
+                filters_are_allowed([modulation])
 
         return value
 
 
 class GroupedMapContentSerializer(ClusterRequestSerializer):
     group_by = serializers.CharField(write_only=True)
```

### Comparing `anycluster-2.3.1/anycluster/api/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.2/anycluster/api/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc` & `anycluster-2.3.2/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/tests/test_views.py` & `anycluster-2.3.2/anycluster/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/urls.py` & `anycluster-2.3.2/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/api/views.py` & `anycluster-2.3.2/anycluster/api/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -257,14 +257,18 @@
 
             return Response(map_content_counts, status=status.HTTP_200_OK)
 
         return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
 
 
 class GetGroupedMapContents(MapClusterViewBase, APIView):
+
+    # hook
+    def prepare_groups(self, groups):
+        return groups
     
     def post(self, request, *args, **kwargs):
         
         serializer = GroupedMapContentSerializer(data=request.data)
 
         if serializer.is_valid():
 
@@ -279,10 +283,12 @@
             group_by = serializer.validated_data['group_by']
 
             map_clusterer = self.get_map_clusterer(geometry_type, CLUSTER_TYPE_KMEANS, filters, clear_cache, output_srid,
                 request, **kwargs)
 
             groups = map_clusterer.get_grouped_map_contents(geojson, geometry_type, zoom, filters, group_by)
 
-            return Response(groups, status=status.HTTP_200_OK)
+            prepared_groups = self.prepare_groups(groups)
+
+            return Response(prepared_groups, status=status.HTTP_200_OK)
             
         return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
```

### Comparing `anycluster-2.3.1/anycluster/clusters.py` & `anycluster-2.3.2/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/definitions.py` & `anycluster-2.3.2/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/globalmaptiles.py` & `anycluster-2.3.2/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/10.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/100.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/1000.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/10000.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/5.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/50.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.3.2/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.2/anycluster/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/__pycache__/mixins.cpython-38.pyc` & `anycluster-2.3.2/anycluster/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc` & `anycluster-2.3.2/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc` & `anycluster-2.3.2/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc` & `anycluster-2.3.2/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc` & `anycluster-2.3.2/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri May 26 08:50:15 2023 UTC, .py size: 25353 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,926 +1,1021 @@
-00000000: 550d 0d0a 0000 0000 c772 7064 0963 0000  U........rpd.c..
+00000000: 550d 0d0a 0000 0000 b213 8764 436b 0000  U..........dCk..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
-00000080: 6d0f 5a0f 6d10 5a10 6d11 5a11 0100 6400  m.Z.m.Z.m.Z...d.
-00000090: 6407 6c12 6d13 5a13 6d14 5a14 6d15 5a15  d.l.m.Z.m.Z.m.Z.
-000000a0: 6d16 5a16 0100 6400 6408 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
+00000020: 0007 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
+00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
+00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000080: 0100 6400 6407 6c0f 6d10 5a10 6d11 5a11  ..d.d.l.m.Z.m.Z.
+00000090: 6d12 5a12 6d13 5a13 6d14 5a14 6d15 5a15  m.Z.m.Z.m.Z.m.Z.
+000000a0: 0100 6400 6408 6c16 6d17 5a17 6d18 5a18  ..d.d.l.m.Z.m.Z.
 000000b0: 6d19 5a19 6d1a 5a1a 0100 6400 6409 6c1b  m.Z.m.Z...d.d.l.
-000000c0: 6d1c 5a1c 0100 6400 640a 6c1d 5a1d 640b  m.Z...d.d.l.Z.d.
-000000d0: 5a1e 640c 5a1f 4700 640d 640e 8400 640e  Z.d.Z.G.d.d...d.
-000000e0: 6519 6518 6501 8305 5a20 4700 640f 6410  e.e.e...Z G.d.d.
-000000f0: 8400 6410 6519 651a 6501 8305 5a21 640a  ..d.e.e.e...Z!d.
-00000100: 5300 2911 e900 0000 0029 01da 0854 6573  S.)......)...Tes
-00000110: 7443 6173 6529 01da 0c47 454f 5347 656f  tCase)...GEOSGeo
-00000120: 6d65 7472 7929 02da 1053 7061 7469 616c  metry)...Spatial
-00000130: 5265 6665 7265 6e63 65da 0e43 6f6f 7264  Reference..Coord
-00000140: 5472 616e 7366 6f72 6d29 01da 0c4d 6170  Transform)...Map
-00000150: 436c 7573 7465 7265 7229 01da 084d 6170  Clusterer)...Map
-00000160: 546f 6f6c 7329 06da 0d43 4c55 5354 4552  Tools)...CLUSTER
-00000170: 5f54 5950 4553 da16 4745 4f4d 4554 5259  _TYPES..GEOMETRY
-00000180: 5f54 5950 455f 5649 4557 504f 5254 da12  _TYPE_VIEWPORT..
-00000190: 4745 4f4d 4554 5259 5f54 5950 455f 4152  GEOMETRY_TYPE_AR
-000001a0: 4541 da0e 4745 4f4d 4554 5259 5f54 5950  EA..GEOMETRY_TYP
-000001b0: 4553 da13 434c 5553 5445 525f 5459 5045  ES..CLUSTER_TYPE
-000001c0: 5f4b 4d45 414e 53da 1143 4c55 5354 4552  _KMEANS..CLUSTER
-000001d0: 5f54 5950 455f 4752 4944 2904 da0f 4745  _TYPE_GRID)...GE
-000001e0: 4f4a 534f 4e5f 504f 4c59 474f 4eda 1147  OJSON_POLYGON..G
-000001f0: 454f 4a53 4f4e 5f52 4543 5441 4e47 4c45  EOJSON_RECTANGLE
-00000200: da14 4745 4f4a 534f 4e5f 4d55 4c54 4950  ..GEOJSON_MULTIP
-00000210: 4f4c 5947 4f4e da19 4745 4f4a 534f 4e5f  OLYGON..GEOJSON_
-00000220: 4645 4154 5552 4543 4f4c 4c45 4354 494f  FEATURECOLLECTIO
-00000230: 4e29 03da 0757 6974 6847 4953 da0b 5769  N)...WithGIS..Wi
-00000240: 7468 4669 6c74 6572 73da 0b57 6974 6847  thFilters..WithG
-00000250: 6172 6465 6e73 2901 da07 4761 7264 656e  ardens)...Garden
-00000260: 734e e907 0000 00e9 0001 0000 6300 0000  sN..........c...
-00000270: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00000280: 0040 0000 0073 bc00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000290: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
-000002a0: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
-000002b0: 5a06 6409 640a 8400 5a07 640b 640c 8400  Z.d.d...Z.d.d...
-000002c0: 5a08 640d 640e 8400 5a09 640f 6410 8400  Z.d.d...Z.d.d...
-000002d0: 5a0a 6411 6412 8400 5a0b 6413 6414 8400  Z.d.d...Z.d.d...
-000002e0: 5a0c 6415 6416 8400 5a0d 6417 6418 8400  Z.d.d...Z.d.d...
-000002f0: 5a0e 6419 641a 8400 5a0f 641b 641c 8400  Z.d.d...Z.d.d...
-00000300: 5a10 641d 641e 8400 5a11 641f 6420 8400  Z.d.d...Z.d.d ..
-00000310: 5a12 6421 6422 8400 5a13 6423 6424 8400  Z.d!d"..Z.d#d$..
-00000320: 5a14 6425 6426 8400 5a15 6427 6428 8400  Z.d%d&..Z.d'd(..
-00000330: 5a16 6429 642a 8400 5a17 642b 642c 8400  Z.d)d*..Z.d+d,..
-00000340: 5a18 642d 5300 292e da10 5465 7374 4d61  Z.d-S.)...TestMa
-00000350: 7043 6c75 7374 6572 6572 6301 0000 0000  pClustererc.....
-00000360: 0000 0000 0000 0008 0000 0009 0000 0043  ...............C
-00000370: 0000 0073 a000 0000 7400 4400 5d96 7d01  ...s....t.D.].}.
-00000380: 7401 4400 5d8c 7d02 7c00 a002 a100 7d03  t.D.].}.|.....}.
-00000390: 7c03 4400 5d7a 7d04 7403 7d05 7c00 a004  |.D.]z}.t.}.|...
-000003a0: 7c02 7c05 7c01 7c04 a104 7d06 7405 7c06  |.|.|.|...}.t.|.
-000003b0: 8301 7d07 7c00 a006 7c07 6a07 7c06 a102  ..}.|...|.j.|...
-000003c0: 0100 7c00 a006 7c07 6a08 6401 a102 0100  ..|...|.j.d.....
-000003d0: 7c00 a006 7c07 6a09 6402 a102 0100 7c00  |...|.j.d.....|.
-000003e0: a006 7c07 6a0a 6403 a102 0100 7c00 a006  ..|.j.d.....|...
-000003f0: 7c07 6a0b 6a0c 740d a102 0100 7c00 a00e  |.j.j.t.....|...
-00000400: 740f 7c07 6a10 7411 8302 a101 0100 711c  t.|.j.t.......q.
-00000410: 710c 7104 6400 5300 2904 4eda 0670 7562  q.q.d.S.).N..pub
-00000420: 6c69 63e9 110f 0000 7217 0000 0029 1272  lic.....r....).r
-00000430: 0800 0000 720b 0000 00da 1067 6574 5f74  ....r......get_t
-00000440: 6573 745f 6669 6c74 6572 73da 0f54 4553  est_filters..TES
-00000450: 545f 5a4f 4f4d 5f4c 4556 454c da11 6765  T_ZOOM_LEVEL..ge
-00000460: 745f 636c 7573 7465 725f 6361 6368 6572  t_cluster_cacher
-00000470: 0600 0000 da0b 6173 7365 7274 4571 7561  ......assertEqua
-00000480: 6cda 0d63 6c75 7374 6572 5f63 6163 6865  l..cluster_cache
-00000490: da0b 7363 6865 6d61 5f6e 616d 65da 0764  ..schema_name..d
-000004a0: 625f 7372 6964 da09 6772 6964 5f73 697a  b_srid..grid_siz
-000004b0: 655a 086d 6170 746f 6f6c 73da 095f 5f63  eZ.maptools..__c
-000004c0: 6c61 7373 5f5f 7207 0000 00da 0a61 7373  lass__r......ass
-000004d0: 6572 7454 7275 65da 0a69 7369 6e73 7461  ertTrue..isinsta
-000004e0: 6e63 655a 0f76 616c 6964 5f6f 7065 7261  nceZ.valid_opera
-000004f0: 746f 7273 da04 6c69 7374 2908 da04 7365  tors..list)...se
-00000500: 6c66 da0b 636c 7573 7465 7274 7970 65da  lf..clustertype.
-00000510: 0d67 656f 6d65 7472 795f 7479 7065 da0c  .geometry_type..
-00000520: 6669 6c74 6572 5f6c 6973 7473 da07 6669  filter_lists..fi
-00000530: 6c74 6572 73da 047a 6f6f 6d72 1f00 0000  lters..zoomr....
-00000540: da0d 6d61 705f 636c 7573 7465 7265 72a9  ..map_clusterer.
-00000550: 0072 2e00 0000 fa46 2f68 6f6d 652f 746f  .r.....F/home/to
-00000560: 6d2f 616e 7963 6c75 7374 6572 2f64 656d  m/anycluster/dem
-00000570: 6f2f 646a 616e 676f 2f61 6e79 636c 7573  o/django/anyclus
-00000580: 7465 722f 7465 7374 732f 7465 7374 5f4d  ter/tests/test_M
-00000590: 6170 436c 7573 7465 7265 722e 7079 da09  apClusterer.py..
-000005a0: 7465 7374 5f69 6e69 7417 0000 0073 1a00  test_init....s..
-000005b0: 0000 0002 0802 0802 0801 0802 0401 1002  ................
-000005c0: 0802 0e01 0e01 0e01 0e01 1001 7a1a 5465  ............z.Te
-000005d0: 7374 4d61 7043 6c75 7374 6572 6572 2e74  stMapClusterer.t
-000005e0: 6573 745f 696e 6974 6301 0000 0000 0000  est_initc.......
-000005f0: 0000 0000 0009 0000 0009 0000 0043 0000  .............C..
-00000600: 0073 5a00 0000 7400 4400 5d50 7d01 7401  .sZ...t.D.]P}.t.
-00000610: 4400 5d46 7d02 7c00 a002 a100 7d03 7c03  D.]F}.|.....}.|.
-00000620: 4400 5d34 7d04 6401 7d05 7c00 a003 7c02  D.]4}.d.}.|...|.
-00000630: 7c05 7c01 7c04 a104 7d06 7404 7c06 8301  |.|.|...}.t.|...
-00000640: 7d07 7c07 a005 a100 7d08 7c00 a006 7c08  }.|.....}.|...|.
-00000650: 6402 a102 0100 711c 710c 7104 6400 5300  d.....q.q.q.d.S.
-00000660: 2903 4ee9 0100 0000 721a 0000 0029 0772  ).N.....r....).r
-00000670: 0800 0000 720b 0000 0072 1b00 0000 721d  ....r....r....r.
-00000680: 0000 0072 0600 0000 5a11 6765 745f 6461  ...r....Z.get_da
-00000690: 7461 6261 7365 5f73 7269 6472 1e00 0000  tabase_sridr....
-000006a0: 2909 7227 0000 0072 2800 0000 7229 0000  ).r'...r(...r)..
-000006b0: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-000006c0: 721f 0000 0072 2d00 0000 7221 0000 0072  r....r-...r!...r
-000006d0: 2e00 0000 722e 0000 0072 2f00 0000 da16  ....r....r/.....
-000006e0: 7465 7374 5f67 6574 5f64 6174 6162 6173  test_get_databas
-000006f0: 655f 7372 6964 2d00 0000 7312 0000 0000  e_srid-...s.....
-00000700: 0208 0208 0208 0108 0204 0110 0208 0208  ................
-00000710: 017a 2754 6573 744d 6170 436c 7573 7465  .z'TestMapCluste
-00000720: 7265 722e 7465 7374 5f67 6574 5f64 6174  rer.test_get_dat
-00000730: 6162 6173 655f 7372 6964 6301 0000 0000  abase_sridc.....
-00000740: 0000 0000 0000 000c 0000 000a 0000 0043  ...............C
-00000750: 0000 0073 d800 0000 7400 4400 5dce 7d01  ...s....t.D.].}.
-00000760: 7401 4400 5dc4 7d02 7c00 a002 a100 7d03  t.D.].}.|.....}.
-00000770: 7c03 4400 5db2 7d04 7403 7d05 7c00 a004  |.D.].}.t.}.|...
-00000780: 7c02 7c05 7c01 7c04 a104 7d06 7405 7c06  |.|.|.|...}.t.|.
-00000790: 8301 7d07 7406 7407 6602 4400 5d46 7d08  ..}.t.t.f.D.]F}.
-000007a0: 7c07 a008 7c08 a101 7d09 7c00 a009 740a  |...|...}.|...t.
-000007b0: 7c09 8301 6401 a102 0100 7c09 4400 5d22  |...d.....|.D.]"
-000007c0: 7d0a 7c00 a00b 740c 7c0a 740d 8302 a101  }.|...t.|.t.....
-000007d0: 0100 7c00 a009 7c0a 6a0e 6402 a102 0100  ..|...|.j.d.....
-000007e0: 7166 7144 7c07 a008 740f a101 7d0b 7c00  qfqD|...t...}.|.
-000007f0: a009 740a 7c0b 8301 6403 a102 0100 7c0b  ..t.|...d.....|.
-00000800: 4400 5d22 7d0a 7c00 a00b 740c 7c0a 740d  D.]"}.|...t.|.t.
-00000810: 8302 a101 0100 7c00 a009 7c0a 6a0e 6402  ......|...|.j.d.
-00000820: a102 0100 71aa 711c 710c 7104 6400 5300  ....q.q.q.q.d.S.
-00000830: 2904 4e72 3100 0000 721a 0000 00e9 0200  ).Nr1...r.......
-00000840: 0000 2910 7208 0000 0072 0b00 0000 721b  ..).r....r....r.
-00000850: 0000 0072 1c00 0000 721d 0000 0072 0600  ...r....r....r..
-00000860: 0000 720e 0000 0072 0f00 0000 5a1f 636f  ..r....r....Z.co
-00000870: 6e76 6572 745f 6765 6f6a 736f 6e5f 6665  nvert_geojson_fe
-00000880: 6174 7572 655f 746f 5f67 656f 7372 1e00  ature_to_geosr..
-00000890: 0000 da03 6c65 6e72 2400 0000 7225 0000  ....lenr$...r%..
-000008a0: 0072 0300 0000 da04 7372 6964 7210 0000  .r......sridr...
-000008b0: 0029 0c72 2700 0000 7228 0000 0072 2900  .).r'...r(...r).
-000008c0: 0000 722a 0000 0072 2b00 0000 722c 0000  ..r*...r+...r,..
-000008d0: 0072 1f00 0000 722d 0000 00da 0767 656f  .r....r-.....geo
-000008e0: 6a73 6f6e da0f 6765 6f73 5f67 656f 6d65  json..geos_geome
-000008f0: 7472 6965 73da 0d67 656f 735f 6765 6f6d  tries..geos_geom
-00000900: 6574 7279 5a12 6d70 5f67 656f 735f 6765  etryZ.mp_geos_ge
-00000910: 6f6d 6574 7269 6573 722e 0000 0072 2e00  ometriesr....r..
-00000920: 0000 722f 0000 00da 2c74 6573 745f 636f  ..r/....,test_co
-00000930: 6e76 6572 745f 6765 6f6a 736f 6e5f 6665  nvert_geojson_fe
-00000940: 6174 7572 655f 746f 5f67 656f 735f 706f  ature_to_geos_po
-00000950: 6c79 676f 6e3f 0000 0073 2c00 0000 0002  lygon?...s,.....
-00000960: 0801 0802 0801 0802 0401 1002 0802 0c02  ................
-00000970: 0401 02ff 0403 1002 0801 1001 1202 0401  ................
-00000980: 02ff 0403 1002 0801 1001 7a3d 5465 7374  ..........z=Test
-00000990: 4d61 7043 6c75 7374 6572 6572 2e74 6573  MapClusterer.tes
-000009a0: 745f 636f 6e76 6572 745f 6765 6f6a 736f  t_convert_geojso
-000009b0: 6e5f 6665 6174 7572 655f 746f 5f67 656f  n_feature_to_geo
-000009c0: 735f 706f 6c79 676f 6e63 0100 0000 0000  s_polygonc......
-000009d0: 0000 0000 0000 0b00 0000 0a00 0000 4300  ..............C.
-000009e0: 0000 737a 0000 0074 0044 005d 707d 0174  ..sz...t.D.]p}.t
-000009f0: 0144 005d 667d 027c 00a0 02a1 007d 037c  .D.]f}.|.....}.|
-00000a00: 0344 005d 547d 0474 037d 057c 00a0 047c  .D.]T}.t.}.|...|
-00000a10: 027c 057c 017c 04a1 047d 0674 057c 0683  .|.|.|...}.t.|..
-00000a20: 017d 0774 0674 0774 0866 0344 005d 287d  .}.t.t.t.f.D.](}
-00000a30: 087c 07a0 097c 08a1 017d 097c 0944 005d  .|...|...}.|.D.]
-00000a40: 147d 0a7c 00a0 0a74 0b7c 0a74 0c83 02a1  .}.|...t.|.t....
-00000a50: 0101 0071 5871 4671 1c71 0c71 0464 0053  ...qXqFq.q.q.d.S
-00000a60: 00a9 014e 290d 7208 0000 0072 0b00 0000  ...N).r....r....
-00000a70: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00000a80: 0600 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00000a90: 0000 00da 1763 6f6e 7665 7274 5f67 656f  .....convert_geo
-00000aa0: 6a73 6f6e 5f74 6f5f 6765 6f73 7224 0000  json_to_geosr$..
-00000ab0: 0072 2500 0000 7203 0000 0029 0b72 2700  .r%...r....).r'.
-00000ac0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-00000ad0: 0072 2b00 0000 722c 0000 0072 1f00 0000  .r+...r,...r....
-00000ae0: 722d 0000 0072 3600 0000 7237 0000 0072  r-...r6...r7...r
-00000af0: 3800 0000 722e 0000 0072 2e00 0000 722f  8...r....r....r/
-00000b00: 0000 00da 2474 6573 745f 636f 6e76 6572  ....$test_conver
-00000b10: 745f 6765 6f6a 736f 6e5f 746f 5f67 656f  t_geojson_to_geo
-00000b20: 735f 6665 6174 7572 6561 0000 0073 1a00  s_featurea...s..
-00000b30: 0000 0002 0801 0802 0801 0802 0401 1002  ................
-00000b40: 0802 0e02 0401 02ff 0403 0801 7a35 5465  ............z5Te
-00000b50: 7374 4d61 7043 6c75 7374 6572 6572 2e74  stMapClusterer.t
-00000b60: 6573 745f 636f 6e76 6572 745f 6765 6f6a  est_convert_geoj
-00000b70: 736f 6e5f 746f 5f67 656f 735f 6665 6174  son_to_geos_feat
-00000b80: 7572 6563 0100 0000 0000 0000 0000 0000  urec............
-00000b90: 0a00 0000 0900 0000 4300 0000 736a 0000  ........C...sj..
-00000ba0: 0074 0044 005d 607d 0174 0144 005d 567d  .t.D.]`}.t.D.]V}
-00000bb0: 027c 00a0 02a1 007d 037c 0344 005d 447d  .|.....}.|.D.]D}
-00000bc0: 0474 037d 057c 00a0 047c 027c 057c 017c  .t.}.|...|.|.|.|
-00000bd0: 04a1 047d 0674 057c 0683 017d 077c 07a0  ...}.t.|...}.|..
-00000be0: 0674 07a1 017d 087c 0844 005d 147d 097c  .t...}.|.D.].}.|
-00000bf0: 00a0 0874 097c 0974 0a83 02a1 0101 0071  ...t.|.t.......q
-00000c00: 4a71 1c71 0c71 0464 0053 0072 3a00 0000  Jq.q.q.d.S.r:...
-00000c10: 290b 7208 0000 0072 0b00 0000 721b 0000  ).r....r....r...
-00000c20: 0072 1c00 0000 721d 0000 0072 0600 0000  .r....r....r....
-00000c30: 723b 0000 0072 1100 0000 7224 0000 0072  r;...r....r$...r
-00000c40: 2500 0000 7203 0000 0029 0a72 2700 0000  %...r....).r'...
-00000c50: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
-00000c60: 2b00 0000 722c 0000 0072 1f00 0000 722d  +...r,...r....r-
-00000c70: 0000 0072 3700 0000 7238 0000 0072 2e00  ...r7...r8...r..
-00000c80: 0000 722e 0000 0072 2f00 0000 da2e 7465  ..r....r/.....te
-00000c90: 7374 5f63 6f6e 7665 7274 5f67 656f 6a73  st_convert_geojs
-00000ca0: 6f6e 5f74 6f5f 6765 6f73 5f66 6561 7475  on_to_geos_featu
-00000cb0: 7265 636f 6c6c 6563 7469 6f6e 7700 0000  recollectionw...
-00000cc0: 7318 0000 0000 0208 0108 0208 0108 0204  s...............
-00000cd0: 0110 0208 0104 0102 ff04 0308 017a 3f54  .............z?T
-00000ce0: 6573 744d 6170 436c 7573 7465 7265 722e  estMapClusterer.
-00000cf0: 7465 7374 5f63 6f6e 7665 7274 5f67 656f  test_convert_geo
-00000d00: 6a73 6f6e 5f74 6f5f 6765 6f73 5f66 6561  json_to_geos_fea
-00000d10: 7475 7265 636f 6c6c 6563 7469 6f6e 6301  turecollectionc.
-00000d20: 0000 0000 0000 0000 0000 000b 0000 000a  ................
-00000d30: 0000 0043 0000 0073 7e00 0000 7400 4400  ...C...s~...t.D.
-00000d40: 5d74 7d01 7401 4400 5d6a 7d02 7c00 a002  ]t}.t.D.]j}.|...
-00000d50: a100 7d03 7c03 4400 5d58 7d04 7403 7d05  ..}.|.D.]X}.t.}.
-00000d60: 7c00 a004 7c02 7c05 7c01 7c04 a104 7d06  |...|.|.|.|...}.
-00000d70: 7405 7c06 8301 7d07 7406 7407 7408 6603  t.|...}.t.t.t.f.
-00000d80: 4400 5d2c 7d08 7c07 a009 7c08 7c02 7c05  D.],}.|...|.|.|.
-00000d90: a103 7d09 7c09 4400 5d14 7d0a 7c00 a00a  ..}.|.D.].}.|...
-00000da0: 740b 7c0a 740c 8302 a101 0100 715c 7146  t.|.t.......q\qF
-00000db0: 711c 710c 7104 6400 5300 723a 0000 0029  q.q.q.d.S.r:...)
-00000dc0: 0d72 0800 0000 720b 0000 0072 1b00 0000  .r....r....r....
-00000dd0: 721c 0000 0072 1d00 0000 7206 0000 0072  r....r....r....r
-00000de0: 0e00 0000 720f 0000 0072 1000 0000 da16  ....r....r......
-00000df0: 6765 745f 636c 7573 7465 725f 6765 6f6d  get_cluster_geom
-00000e00: 6574 7269 6573 7224 0000 0072 2500 0000  etriesr$...r%...
-00000e10: 7203 0000 0029 0b72 2700 0000 7228 0000  r....).r'...r(..
-00000e20: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
-00000e30: 722c 0000 0072 1f00 0000 722d 0000 0072  r,...r....r-...r
-00000e40: 3600 0000 da12 636c 7573 7465 725f 6765  6.....cluster_ge
-00000e50: 6f6d 6574 7269 6573 7238 0000 0072 2e00  ometriesr8...r..
-00000e60: 0000 722e 0000 0072 2f00 0000 da24 7465  ..r....r/....$te
-00000e70: 7374 5f67 6574 5f63 6c75 7374 6572 5f67  st_get_cluster_g
-00000e80: 656f 6d65 7472 6965 735f 7669 6577 706f  eometries_viewpo
-00000e90: 7274 8a00 0000 731e 0000 0000 0208 0108  rt....s.........
-00000ea0: 0308 0108 0204 0110 0208 020e 0204 0102  ................
-00000eb0: 0002 0002 ff04 0308 017a 3554 6573 744d  .........z5TestM
-00000ec0: 6170 436c 7573 7465 7265 722e 7465 7374  apClusterer.test
-00000ed0: 5f67 6574 5f63 6c75 7374 6572 5f67 656f  _get_cluster_geo
-00000ee0: 6d65 7472 6965 735f 7669 6577 706f 7274  metries_viewport
-00000ef0: 6301 0000 0000 0000 0000 0000 000d 0000  c...............
-00000f00: 0009 0000 0043 0000 0073 d600 0000 7400  .....C...s....t.
-00000f10: 4400 5dcc 7d01 7c00 a001 a100 7d02 7c02  D.].}.|.....}.|.
-00000f20: 4400 5dba 7d03 7402 7d04 7c00 a003 7404  D.].}.t.}.|...t.
-00000f30: 7c04 7c01 7c03 a104 7d05 7405 7c05 8301  |.|.|...}.t.|...
-00000f40: 7d06 7406 7d07 7c06 a007 7c07 7404 7c04  }.t.}.|...|.t.|.
-00000f50: a103 7d08 7406 6401 1900 a008 a100 7d09  ..}.t.d.......}.
-00000f60: 7409 740a a00b 7c09 a101 6402 6403 8d02  t.t...|...d.d...
-00000f70: 7d0a 740c 740d 7c0a 6a0e 8301 740d 6404  }.t.t.|.j...t.d.
-00000f80: 8301 8302 7d0b 7c0a a00f 7c0b a101 0100  ....}.|...|.....
-00000f90: 7c00 a010 7c0a 6a11 7c08 6405 1900 6a11  |...|.j.|.d...j.
-00000fa0: a102 0100 7412 7406 7413 6603 4400 5d2c  ....t.t.t.f.D.],
-00000fb0: 7d07 7c06 a007 7c07 7404 7c04 a103 7d08  }.|...|.t.|...}.
-00000fc0: 7c08 4400 5d14 7d0c 7c00 a014 7415 7c0c  |.D.].}.|...t.|.
-00000fd0: 7409 8302 a101 0100 71b6 71a0 7114 7104  t.......q.q.q.q.
-00000fe0: 6400 5300 2906 4eda 0867 656f 6d65 7472  d.S.).N..geometr
-00000ff0: 79e9 e610 0000 2901 7235 0000 0072 1a00  y.....).r5...r..
-00001000: 0000 7201 0000 0029 1672 0800 0000 721b  ..r....).r....r.
-00001010: 0000 0072 1c00 0000 721d 0000 0072 0a00  ...r....r....r..
-00001020: 0000 7206 0000 0072 0f00 0000 723e 0000  ..r....r....r>..
-00001030: 00da 0463 6f70 7972 0300 0000 da04 6a73  ...copyr......js
-00001040: 6f6e da05 6475 6d70 7372 0500 0000 7204  on..dumpsr....r.
-00001050: 0000 0072 3500 0000 da09 7472 616e 7366  ...r5.....transf
-00001060: 6f72 6d72 1e00 0000 7236 0000 0072 0e00  ormr....r6...r..
-00001070: 0000 7210 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
-00001080: 0029 0d72 2700 0000 7228 0000 0072 2a00  .).r'...r(...r*.
-00001090: 0000 722b 0000 0072 2c00 0000 721f 0000  ..r+...r,...r...
-000010a0: 0072 2d00 0000 7236 0000 0072 3f00 0000  .r-...r6...r?...
-000010b0: 5a10 6d61 7463 6869 6e67 5f67 656f 6a73  Z.matching_geojs
-000010c0: 6f6e 5a0c 696e 6974 6961 6c5f 6765 6f73  onZ.initial_geos
-000010d0: da02 6374 7238 0000 0072 2e00 0000 722e  ..ctr8...r....r.
-000010e0: 0000 0072 2f00 0000 da20 7465 7374 5f67  ...r/.... test_g
-000010f0: 6574 5f63 6c75 7374 6572 5f67 656f 6d65  et_cluster_geome
-00001100: 7472 6965 735f 6172 6561 a100 0000 7344  tries_area....sD
-00001110: 0000 0000 0208 0308 0108 0204 0110 0208  ................
-00001120: 0204 0204 0102 0002 0002 ff04 030c 0102  ................
-00001130: 0108 0002 ff06 0204 0104 ff02 0106 ff04  ................
-00001140: 020a 0208 0108 ff04 030e 0204 0102 0002  ................
-00001150: 0002 ff04 0308 017a 3154 6573 744d 6170  .......z1TestMap
-00001160: 436c 7573 7465 7265 722e 7465 7374 5f67  Clusterer.test_g
-00001170: 6574 5f63 6c75 7374 6572 5f67 656f 6d65  et_cluster_geome
-00001180: 7472 6965 735f 6172 6561 6301 0000 0000  tries_areac.....
-00001190: 0000 0000 0000 0009 0000 0009 0000 0043  ...............C
-000011a0: 0000 0073 7a00 0000 7400 7d01 7401 4400  ...sz...t.}.t.D.
-000011b0: 5d6c 7d02 7402 7403 7404 6603 4400 5d5c  ]l}.t.t.t.f.D.]\
-000011c0: 7d03 7c00 a005 a100 7d04 7c04 4400 5d4a  }.|.....}.|.D.]J
-000011d0: 7d05 7c00 a006 7c02 7c01 7407 7c05 a104  }.|...|.|.t.|...
-000011e0: 7d06 7408 7c06 8301 7d07 6700 7d05 7c07  }.t.|...}.g.}.|.
-000011f0: a009 7c03 7c02 7c01 7c05 a104 7d08 7c02  ..|.|.|.|...}.|.
-00001200: 740a 6b02 7226 7c00 a00b 740c 7c08 8301  t.k.r&|...t.|...
-00001210: 6401 6b04 a101 0100 7126 7116 7108 6400  d.k.....q&q.q.d.
-00001220: 5300 a902 4e72 0100 0000 290d 721c 0000  S...Nr....).r...
-00001230: 0072 0b00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00001240: 7210 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
-00001250: 0c00 0000 7206 0000 00da 0e6b 6d65 616e  ....r......kmean
-00001260: 735f 636c 7573 7465 7272 0900 0000 7224  s_clusterr....r$
-00001270: 0000 0072 3400 0000 2909 7227 0000 0072  ...r4...).r'...r
-00001280: 2c00 0000 7229 0000 0072 3600 0000 722a  ,...r)...r6...r*
-00001290: 0000 0072 2b00 0000 721f 0000 0072 2d00  ...r+...r....r-.
-000012a0: 0000 da07 6d61 726b 6572 7372 2e00 0000  ....markersr....
-000012b0: 722e 0000 0072 2f00 0000 da13 7465 7374  r....r/.....test
-000012c0: 5f6b 6d65 616e 735f 636c 7573 7465 72c6  _kmeans_cluster.
-000012d0: 0000 0073 1600 0000 0002 0402 0801 0e03  ...s............
-000012e0: 0801 0802 1002 0802 0402 1002 0801 7a24  ..............z$
-000012f0: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
-00001300: 2e74 6573 745f 6b6d 6561 6e73 5f63 6c75  .test_kmeans_clu
-00001310: 7374 6572 6301 0000 0000 0000 0000 0000  sterc...........
-00001320: 000a 0000 0009 0000 0043 0000 0073 6a00  .........C...sj.
-00001330: 0000 7400 7d01 7401 4400 5d5c 7d02 7402  ..t.}.t.D.]\}.t.
-00001340: 4400 5d52 7d03 7c00 a003 a100 7d04 7c04  D.]R}.|.....}.|.
-00001350: 4400 5d40 7d05 7c00 a004 7c03 7c01 7c02  D.]@}.|...|.|.|.
-00001360: 7c05 a104 7d06 7405 7c06 8301 7d07 7406  |...}.t.|...}.t.
-00001370: 7407 6602 4400 5d1a 7d08 7c07 a008 7c08  t.f.D.].}.|...|.
-00001380: a101 7d09 7c00 a009 7c09 6401 a102 0100  ..}.|...|.d.....
-00001390: 7144 7120 7110 7108 6400 5300 2902 4e72  qDq q.q.d.S.).Nr
-000013a0: 4200 0000 290a 721c 0000 0072 0800 0000  B...).r....r....
-000013b0: 720b 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
-000013c0: 0600 0000 720e 0000 0072 0f00 0000 5a1d  ....r....r....Z.
-000013d0: 6765 745f 7372 6964 5f66 726f 6d5f 6765  get_srid_from_ge
-000013e0: 6f6a 736f 6e5f 6665 6174 7572 6572 1e00  ojson_featurer..
-000013f0: 0000 290a 7227 0000 0072 2c00 0000 7228  ..).r'...r,...r(
-00001400: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
-00001410: 0000 721f 0000 0072 2d00 0000 7236 0000  ..r....r-...r6..
-00001420: 0072 3500 0000 722e 0000 0072 2e00 0000  .r5...r....r....
-00001430: 722f 0000 00da 2274 6573 745f 6765 745f  r/...."test_get_
-00001440: 7372 6964 5f66 726f 6d5f 6765 6f6a 736f  srid_from_geojso
-00001450: 6e5f 6665 6174 7572 65dd 0000 0073 1400  n_feature....s..
-00001460: 0000 0002 0402 0801 0802 0801 0802 1002  ................
-00001470: 0802 0c02 0a02 7a33 5465 7374 4d61 7043  ......z3TestMapC
-00001480: 6c75 7374 6572 6572 2e74 6573 745f 6765  lusterer.test_ge
-00001490: 745f 7372 6964 5f66 726f 6d5f 6765 6f6a  t_srid_from_geoj
-000014a0: 736f 6e5f 6665 6174 7572 6563 0100 0000  son_featurec....
-000014b0: 0000 0000 0000 0000 0800 0000 0700 0000  ................
-000014c0: 4300 0000 735a 0000 007c 00a0 00a1 007d  C...sZ...|.....}
-000014d0: 017c 0144 005d 487d 0274 017d 037c 00a0  .|.D.]H}.t.}.|..
-000014e0: 0274 037c 0374 047c 02a1 047d 0474 057c  .t.|.t.|...}.t.|
-000014f0: 0483 017d 0567 007d 0274 067d 067c 05a0  ...}.g.}.t.}.|..
-00001500: 077c 067c 037c 02a1 037d 077c 00a0 0874  .|.|.|...}.|...t
-00001510: 097c 0783 0164 016b 04a1 0101 0071 0c64  .|...d.k.....q.d
-00001520: 0053 0072 4900 0000 290a 721b 0000 0072  .S.rI...).r....r
-00001530: 1c00 0000 721d 0000 0072 0900 0000 720d  ....r....r....r.
-00001540: 0000 0072 0600 0000 720f 0000 005a 0c67  ...r....r....Z.g
-00001550: 7269 645f 636c 7573 7465 7272 2400 0000  rid_clusterr$...
-00001560: 7234 0000 0029 0872 2700 0000 722a 0000  r4...).r'...r*..
-00001570: 0072 2b00 0000 722c 0000 0072 1f00 0000  .r+...r,...r....
-00001580: 722d 0000 0072 3600 0000 da05 6365 6c6c  r-...r6.....cell
-00001590: 7372 2e00 0000 722e 0000 0072 2f00 0000  sr....r....r/...
-000015a0: da11 7465 7374 5f67 7269 645f 636c 7573  ..test_grid_clus
-000015b0: 7465 72f2 0000 0073 1200 0000 0002 0801  ter....s........
-000015c0: 0802 0401 1002 0802 0402 0402 0e02 7a22  ..............z"
-000015d0: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
-000015e0: 2e74 6573 745f 6772 6964 5f63 6c75 7374  .test_grid_clust
-000015f0: 6572 6301 0000 0000 0000 0000 0000 000a  erc.............
-00001600: 0000 000a 0000 0043 0000 0073 6c00 0000  .......C...sl...
-00001610: 7400 7d01 7401 4400 5d5e 7d02 7402 4400  t.}.t.D.]^}.t.D.
-00001620: 5d54 7d03 7c00 a003 a100 7d04 7c04 4400  ]T}.|.....}.|.D.
-00001630: 5d42 7d05 7c00 a004 7c03 7c01 7c02 7c05  ]B}.|...|.|.|.|.
-00001640: a104 7d06 7405 7c06 8301 7d07 7c07 a006  ..}.t.|...}.|...
-00001650: a100 7d08 6401 6402 6403 6404 6405 6406  ..}.d.d.d.d.d.d.
-00001660: 6407 6707 7d09 7c00 a007 7c08 7c09 a102  d.g.}.|...|.|...
-00001670: 0100 7120 7110 7108 6400 5300 2908 4eda  ..q q.q.d.S.).N.
-00001680: 0269 64da 046e 616d 65da 0573 7479 6c65  .id..name..style
-00001690: da06 7261 7469 6e67 da0d 6672 6565 5f65  ..rating..free_e
-000016a0: 6e74 7261 6e63 65da 0c6c 6173 745f 7265  ntrance..last_re
-000016b0: 6e65 7761 6cfa 1263 6f6f 7264 696e 6174  newal..coordinat
-000016c0: 6573 3a3a 6279 7465 6129 0872 1c00 0000  es::bytea).r....
-000016d0: 7208 0000 0072 0b00 0000 721b 0000 0072  r....r....r....r
-000016e0: 1d00 0000 7206 0000 00da 1367 6574 5f67  ....r......get_g
-000016f0: 6973 5f66 6965 6c64 5f6e 616d 6573 721e  is_field_namesr.
-00001700: 0000 0029 0a72 2700 0000 722c 0000 0072  ...).r'...r,...r
-00001710: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
-00001720: 0000 0072 1f00 0000 722d 0000 00da 0b66  ...r....r-.....f
-00001730: 6965 6c64 5f6e 616d 6573 5a14 6578 7065  ield_namesZ.expe
-00001740: 6374 6564 5f66 6965 6c64 5f6e 616d 6573  cted_field_names
-00001750: 722e 0000 0072 2e00 0000 722f 0000 00da  r....r....r/....
-00001760: 1874 6573 745f 6765 745f 6769 735f 6669  .test_get_gis_fi
-00001770: 656c 645f 6e61 6d65 7305 0100 0073 1800  eld_names....s..
-00001780: 0000 0002 0402 0801 0802 0801 0802 1002  ................
-00001790: 0802 0802 0c01 02ff 0403 7a29 5465 7374  ..........z)Test
-000017a0: 4d61 7043 6c75 7374 6572 6572 2e74 6573  MapClusterer.tes
-000017b0: 745f 6765 745f 6769 735f 6669 656c 645f  t_get_gis_field_
-000017c0: 6e61 6d65 7363 0100 0000 0000 0000 0000  namesc..........
-000017d0: 0000 0a00 0000 0900 0000 4300 0000 735e  ..........C...s^
-000017e0: 0000 0074 007d 0174 0144 005d 507d 0274  ...t.}.t.D.]P}.t
-000017f0: 0244 005d 467d 037c 00a0 03a1 007d 047c  .D.]F}.|.....}.|
-00001800: 0444 005d 347d 057c 00a0 047c 037c 017c  .D.]4}.|...|.|.|
-00001810: 027c 05a1 047d 0674 057c 0683 017d 077c  .|...}.t.|...}.|
-00001820: 07a0 06a1 007d 0864 017d 097c 00a0 077c  .....}.d.}.|...|
-00001830: 087c 09a1 0201 0071 2071 1071 0864 0053  .|.....q q.q.d.S
-00001840: 0029 024e 7a42 6964 2c6e 616d 652c 7374  .).NzBid,name,st
-00001850: 796c 652c 7261 7469 6e67 2c66 7265 655f  yle,rating,free_
-00001860: 656e 7472 616e 6365 2c6c 6173 745f 7265  entrance,last_re
-00001870: 6e65 7761 6c2c 636f 6f72 6469 6e61 7465  newal,coordinate
-00001880: 733a 3a62 7974 6561 2908 721c 0000 0072  s::bytea).r....r
-00001890: 0800 0000 720b 0000 0072 1b00 0000 721d  ....r....r....r.
-000018a0: 0000 0072 0600 0000 5a12 6765 745f 6769  ...r....Z.get_gi
-000018b0: 735f 6669 656c 6473 5f73 7472 721e 0000  s_fields_strr...
-000018c0: 0029 0a72 2700 0000 722c 0000 0072 2800  .).r'...r,...r(.
-000018d0: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
-000018e0: 0072 1f00 0000 722d 0000 005a 0a66 6965  .r....r-...Z.fie
-000018f0: 6c64 735f 7374 725a 0c65 7870 6563 7465  lds_strZ.expecte
-00001900: 645f 7374 7272 2e00 0000 722e 0000 0072  d_strr....r....r
-00001910: 2f00 0000 da16 7465 7374 5f67 6574 5f67  /.....test_get_g
-00001920: 6973 5f66 6965 6c64 5f73 7472 1b01 0000  is_field_str....
-00001930: 7314 0000 0000 0204 0208 0108 0308 0108  s...............
-00001940: 0210 0208 0208 0104 027a 2754 6573 744d  .........z'TestM
-00001950: 6170 436c 7573 7465 7265 722e 7465 7374  apClusterer.test
-00001960: 5f67 6574 5f67 6973 5f66 6965 6c64 5f73  _get_gis_field_s
-00001970: 7472 6301 0000 0000 0000 0000 0000 000f  trc.............
-00001980: 0000 000b 0000 0043 0000 0073 f200 0000  .......C...s....
-00001990: 6401 7d01 7400 4400 5de4 7d02 7401 4400  d.}.t.D.].}.t.D.
-000019a0: 5dda 7d03 7c00 a002 a100 7d04 7c04 4400  ].}.|.....}.|.D.
-000019b0: 5dc8 7d05 7c00 a003 7c03 7c01 7c02 7c05  ].}.|...|.|.|.|.
-000019c0: a104 7d06 7404 7c06 8301 7d07 7405 7d08  ..}.t.|...}.t.}.
-000019d0: 6700 7d05 7c07 a006 7c08 7c03 7c01 7c05  g.}.|...|.|.|.|.
-000019e0: a104 7d09 7c03 7407 6b02 7270 7c00 a008  ..}.|.t.k.rp|...
-000019f0: 7409 7c07 6a0a 6a0b 8301 6401 a102 0100  t.|.j.j...d.....
-00001a00: 7c00 a00c 7409 7c09 8301 6402 6b04 a101  |...t.|...d.k...
-00001a10: 0100 7c09 6402 1900 7d0a 7c0a 6403 1900  ..|.d...}.|.d...
-00001a20: 7d0b 7c0a 6404 1900 6405 1900 7d0c 7c0a  }.|.d...d...}.|.
-00001a30: 6404 1900 6406 1900 7d0d 7c07 a00d 7c03  d...d...}.|...|.
-00001a40: 7c0b 7c0c 7c0d 7c05 7c01 a106 7d0e 7c00  |.|.|.|.|...}.|.
-00001a50: a00c 7c0a 6407 1900 6402 6b04 a101 0100  ..|.d...d.k.....
-00001a60: 7c00 a008 7409 740e 7c0e 8301 8301 7c0a  |...t.t.|.....|.
-00001a70: 6407 1900 a102 0100 7120 7110 7108 6400  d.......q q.q.d.
-00001a80: 5300 2908 4e72 3100 0000 7201 0000 00da  S.).Nr1...r.....
-00001a90: 0369 6473 da06 6365 6e74 6572 da01 78da  .ids..center..x.
-00001aa0: 0179 da05 636f 756e 7429 0f72 0800 0000  .y..count).r....
-00001ab0: 720b 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
-00001ac0: 0600 0000 720f 0000 0072 4a00 0000 720a  ....r....rJ...r.
-00001ad0: 0000 0072 1e00 0000 7234 0000 0072 1f00  ...r....r4...r..
-00001ae0: 0000 da0a 6765 6f6d 6574 7269 6573 7224  ....geometriesr$
-00001af0: 0000 005a 1a67 6574 5f6b 6d65 616e 735f  ...Z.get_kmeans_
-00001b00: 636c 7573 7465 725f 636f 6e74 656e 7472  cluster_contentr
-00001b10: 2600 0000 290f 7227 0000 0072 2c00 0000  &...).r'...r,...
-00001b20: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
-00001b30: 2b00 0000 721f 0000 0072 2d00 0000 7236  +...r....r-...r6
-00001b40: 0000 0072 4b00 0000 da06 6d61 726b 6572  ...rK.....marker
-00001b50: 725b 0000 0072 5d00 0000 725e 0000 005a  r[...r]...r^...Z
-00001b60: 0f63 6c75 7374 6572 5f63 6f6e 7465 6e74  .cluster_content
-00001b70: 722e 0000 0072 2e00 0000 722f 0000 00da  r....r....r/....
-00001b80: 1f74 6573 745f 6765 745f 6b6d 6561 6e73  .test_get_kmeans
-00001b90: 5f63 6c75 7374 6572 5f63 6f6e 7465 6e74  _cluster_content
-00001ba0: 3001 0000 7328 0000 0000 0204 0208 0108  0...s(..........
-00001bb0: 0308 0108 0210 0208 0204 0204 0210 0208  ................
-00001bc0: 0114 0212 0208 0208 010c 010c 0214 0212  ................
-00001bd0: 017a 3054 6573 744d 6170 436c 7573 7465  .z0TestMapCluste
-00001be0: 7265 722e 7465 7374 5f67 6574 5f6b 6d65  rer.test_get_kme
-00001bf0: 616e 735f 636c 7573 7465 725f 636f 6e74  ans_cluster_cont
-00001c00: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
-00001c10: 0a00 0000 0900 0000 4300 0000 736e 0000  ........C...sn..
-00001c20: 0064 017d 0174 0044 005d 607d 0274 0144  .d.}.t.D.]`}.t.D
-00001c30: 005d 567d 037c 00a0 02a1 007d 047c 0444  .]V}.|.....}.|.D
-00001c40: 005d 447d 057c 00a0 037c 037c 017c 027c  .]D}.|...|.|.|.|
-00001c50: 05a1 047d 0674 047c 0683 017d 0774 057d  ...}.t.|...}.t.}
-00001c60: 0867 007d 057c 07a0 067c 087c 05a1 027d  .g.}.|...|.|...}
-00001c70: 097c 00a0 0774 0874 097c 0983 0183 0164  .|...t.t.|.....d
-00001c80: 02a1 0201 0071 2071 1071 0864 0053 0029  .....q q.q.d.S.)
-00001c90: 034e 7231 0000 00e9 6400 0000 290a 7208  .Nr1....d...).r.
-00001ca0: 0000 0072 0b00 0000 721b 0000 0072 1d00  ...r....r....r..
-00001cb0: 0000 7206 0000 0072 0f00 0000 5a10 6765  ..r....r....Z.ge
-00001cc0: 745f 6172 6561 5f63 6f6e 7465 6e74 721e  t_area_contentr.
-00001cd0: 0000 0072 3400 0000 7226 0000 0029 0a72  ...r4...r&...).r
-00001ce0: 2700 0000 722c 0000 0072 2800 0000 7229  '...r,...r(...r)
-00001cf0: 0000 0072 2a00 0000 722b 0000 0072 1f00  ...r*...r+...r..
-00001d00: 0000 722d 0000 0072 3600 0000 5a0c 6172  ..r-...r6...Z.ar
-00001d10: 6561 5f63 6f6e 7465 6e74 722e 0000 0072  ea_contentr....r
-00001d20: 2e00 0000 722f 0000 00da 1574 6573 745f  ....r/.....test_
-00001d30: 6765 745f 6172 6561 5f63 6f6e 7465 6e74  get_area_content
-00001d40: 5601 0000 7316 0000 0000 0204 0208 0108  V...s...........
-00001d50: 0308 0108 0210 0208 0204 0104 020c 027a  ...............z
-00001d60: 2654 6573 744d 6170 436c 7573 7465 7265  &TestMapClustere
-00001d70: 722e 7465 7374 5f67 6574 5f61 7265 615f  r.test_get_area_
-00001d80: 636f 6e74 656e 7463 0100 0000 0000 0000  contentc........
-00001d90: 0000 0000 0b00 0000 0900 0000 4300 0000  ............C...
-00001da0: 7364 0000 0064 017d 0174 0044 005d 567d  sd...d.}.t.D.]V}
-00001db0: 0274 0144 005d 4c7d 037c 00a0 02a1 007d  .t.D.]L}.|.....}
-00001dc0: 047c 0444 005d 3a7d 057c 00a0 037c 037c  .|.D.]:}.|...|.|
-00001dd0: 017c 027c 05a1 047d 0674 047c 0683 017d  .|.|...}.t.|...}
-00001de0: 0774 057d 087c 07a0 067c 08a1 017d 0964  .t.}.|...|...}.d
-00001df0: 027d 0a7c 00a0 077c 097c 0aa1 0201 0071  .}.|...|.|.....q
-00001e00: 2071 1071 0864 0053 0029 034e 7231 0000   q.q.d.S.).Nr1..
-00001e10: 0061 0301 0000 2820 5354 5f49 6e74 6572  .a....( ST_Inter
-00001e20: 7365 6374 7328 636f 6f72 6469 6e61 7465  sects(coordinate
-00001e30: 732c 2053 545f 4765 6f6d 6574 7279 4672  s, ST_GeometryFr
-00001e40: 6f6d 5465 7874 2827 504f 4c59 474f 4e20  omText('POLYGON 
-00001e50: 2828 3939 3038 3532 2e35 3438 3139 3339  ((990852.5481939
-00001e60: 3934 3120 3635 3339 3635 302e 3638 3930  941 6539650.6890
-00001e70: 3732 3839 392c 2039 3930 3835 322e 3534  72899, 990852.54
-00001e80: 3831 3933 3939 3431 2035 3938 3032 3237  81939941 5980227
-00001e90: 2e31 3032 3032 3834 3238 2c20 3135 3539  .102028428, 1559
-00001ea0: 3837 362e 3232 3739 3935 3930 3238 2035  876.2279959028 5
-00001eb0: 3938 3032 3237 2e31 3032 3032 3834 3238  980227.102028428
-00001ec0: 2c20 3135 3539 3837 362e 3232 3739 3935  , 1559876.227995
-00001ed0: 3930 3238 2036 3533 3936 3530 2e36 3839  9028 6539650.689
-00001ee0: 3037 3238 3939 2c20 3939 3038 3532 2e35  072899, 990852.5
-00001ef0: 3438 3139 3339 3934 3120 3635 3339 3635  481939941 653965
-00001f00: 302e 3638 3930 3732 3839 3929 2927 2c20  0.689072899))', 
-00001f10: 3338 3537 2920 2920 2929 0872 0800 0000  3857) ) )).r....
-00001f20: 720b 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
-00001f30: 0600 0000 720f 0000 005a 1567 6574 5f67  ....r....Z.get_g
-00001f40: 656f 6d5f 6669 6c74 6572 7374 7269 6e67  eom_filterstring
-00001f50: 721e 0000 0029 0b72 2700 0000 722c 0000  r....).r'...r,..
-00001f60: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
-00001f70: 722b 0000 0072 1f00 0000 722d 0000 0072  r+...r....r-...r
-00001f80: 3600 0000 5a11 6765 6f6d 5f66 696c 7465  6...Z.geom_filte
-00001f90: 7273 7472 696e 675a 0f65 7870 6563 7465  rstringZ.expecte
-00001fa0: 645f 7374 7269 6e67 722e 0000 0072 2e00  d_stringr....r..
-00001fb0: 0000 722f 0000 00da 1a74 6573 745f 6765  ..r/.....test_ge
-00001fc0: 745f 6765 6f6d 5f66 696c 7465 7273 7472  t_geom_filterstr
-00001fd0: 696e 676d 0100 0073 1600 0000 0002 0402  ingm...s........
-00001fe0: 0801 0803 0801 0802 1002 0802 0402 0a02  ................
-00001ff0: 0402 7a2b 5465 7374 4d61 7043 6c75 7374  ..z+TestMapClust
-00002000: 6572 6572 2e74 6573 745f 6765 745f 6765  erer.test_get_ge
-00002010: 6f6d 5f66 696c 7465 7273 7472 696e 6763  om_filterstringc
-00002020: 0100 0000 0000 0000 0000 0000 0c00 0000  ................
-00002030: 0900 0000 4300 0000 7388 0000 0064 017d  ....C...s....d.}
-00002040: 0174 0044 005d 7a7d 0274 0144 005d 707d  .t.D.]z}.t.D.]p}
-00002050: 037c 00a0 02a1 007d 047c 0444 005d 5e7d  .|.....}.|.D.]^}
-00002060: 057c 00a0 037c 037c 017c 027c 05a1 047d  .|...|.|.|.|...}
-00002070: 0674 047c 0683 017d 0774 057d 087c 07a0  .t.|...}.t.}.|..
-00002080: 067c 0864 027c 01a1 037d 097c 00a0 0774  .|.d.|...}.|...t
-00002090: 087c 0983 0164 03a1 0201 007c 0964 0419  .|...d.....|.d..
-000020a0: 007d 0a7c 07a0 097c 0a7c 01a1 027d 0b7c  .}.|...|.|...}.|
-000020b0: 00a0 077c 0b64 05a1 0201 0071 2071 1071  ...|.d.....q q.q
-000020c0: 0864 0053 0029 064e e90a 0000 00da 0461  .d.S.).N.......a
-000020d0: 7265 6172 3100 0000 7201 0000 00e9 1e00  rear1...r.......
-000020e0: 0000 290a 7208 0000 0072 0b00 0000 721b  ..).r....r....r.
-000020f0: 0000 0072 1d00 0000 7206 0000 0072 0e00  ...r....r....r..
-00002100: 0000 723e 0000 0072 1e00 0000 7234 0000  ..r>...r....r4..
-00002110: 005a 0b63 616c 6375 6c61 7465 5f6b 290c  .Z.calculate_k).
-00002120: 7227 0000 0072 2c00 0000 7228 0000 0072  r'...r,...r(...r
-00002130: 2900 0000 722a 0000 0072 2b00 0000 721f  )...r*...r+...r.
-00002140: 0000 0072 2d00 0000 7236 0000 0072 3700  ...r-...r6...r7.
-00002150: 0000 da04 6765 6f73 da01 6b72 2e00 0000  ....geos..kr....
-00002160: 722e 0000 0072 2f00 0000 da10 7465 7374  r....r/.....test
-00002170: 5f63 616c 6375 6c61 7465 5f6b 8501 0000  _calculate_k....
-00002180: 731a 0000 0000 0204 0208 0108 0208 0108  s...............
-00002190: 0210 0208 0204 020e 0210 0208 020c 027a  ...............z
-000021a0: 2154 6573 744d 6170 436c 7573 7465 7265  !TestMapClustere
-000021b0: 722e 7465 7374 5f63 616c 6375 6c61 7465  r.test_calculate
-000021c0: 5f6b 6301 0000 0000 0000 0000 0000 000b  _kc.............
-000021d0: 0000 0009 0000 0043 0000 0073 c800 0000  .......C...s....
-000021e0: 7400 7d01 7401 4400 5dba 7d02 7402 4400  t.}.t.D.].}.t.D.
-000021f0: 5db0 7d03 7c00 a003 a100 7d04 7c04 4400  ].}.|.....}.|.D.
-00002200: 5d9e 7d05 7c00 a004 7c02 7c01 7c03 7c05  ].}.|...|.|.|.|.
-00002210: a104 7d06 7405 7c06 8301 7d07 7406 7d08  ..}.t.|...}.t.}.
-00002220: 7c07 a007 7c08 7c02 7c01 a103 7d09 7c00  |...|.|.|...}.|.
-00002230: a008 7409 7c09 8301 6401 6b04 a101 0100  ..t.|...d.k.....
-00002240: 7c00 a00a 7c07 6a0b 6a0c 7c01 a102 0100  |...|.j.j.|.....
-00002250: 7c00 a00a 7c07 6a0b 6a0d 7c03 a102 0100  |...|.j.j.|.....
-00002260: 7c00 a00a 7c07 6a0b 6a0e 7c02 a102 0100  |...|.j.j.|.....
-00002270: 7c00 a00a 7c07 6a0b 6a0f 7c05 a102 0100  |...|.j.j.|.....
-00002280: 7c07 a007 7c08 7c02 7c01 a103 7d0a 7c00  |...|.|.|...}.|.
-00002290: a00a 7409 7c0a 8301 6401 a102 0100 7120  ..t.|...d.....q 
-000022a0: 7110 7108 6400 5300 7249 0000 0029 1072  q.q.d.S.rI...).r
-000022b0: 1c00 0000 720b 0000 0072 0800 0000 721b  ....r....r....r.
-000022c0: 0000 0072 1d00 0000 7206 0000 0072 0f00  ...r....r....r..
-000022d0: 0000 723e 0000 0072 2400 0000 7234 0000  ..r>...r$...r4..
-000022e0: 0072 1e00 0000 721f 0000 0072 2c00 0000  .r....r....r,...
-000022f0: 7228 0000 0072 2900 0000 722b 0000 0029  r(...r)...r+...)
-00002300: 0b72 2700 0000 722c 0000 0072 2900 0000  .r'...r,...r)...
-00002310: 7228 0000 0072 2a00 0000 722b 0000 0072  r(...r*...r+...r
-00002320: 1f00 0000 722d 0000 0072 3600 0000 723f  ....r-...r6...r?
-00002330: 0000 005a 1863 6163 6865 5f63 6c75 7374  ...Z.cache_clust
-00002340: 6572 5f67 656f 6d65 7472 6965 7372 2e00  er_geometriesr..
-00002350: 0000 722e 0000 0072 2f00 0000 da17 7465  ..r....r/.....te
-00002360: 7374 5f73 616d 655f 7265 7175 6573 745f  st_same_request_
-00002370: 7477 6963 65a0 0100 0073 3000 0000 0002  twice....s0.....
-00002380: 0402 0801 0803 0801 0802 1002 0802 0402  ................
-00002390: 0401 0200 0200 02ff 0403 1201 1001 1001  ................
-000023a0: 1001 1002 0401 0200 0200 02ff 0403 7a28  ..............z(
-000023b0: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
-000023c0: 2e74 6573 745f 7361 6d65 5f72 6571 7565  .test_same_reque
-000023d0: 7374 5f74 7769 6365 6301 0000 0000 0000  st_twicec.......
-000023e0: 0000 0000 0008 0000 0008 0000 0043 0000  .............C..
-000023f0: 0073 7e00 0000 7400 6a01 a002 a100 a003  .s~...t.j.......
-00002400: a100 7d01 7c00 a004 a100 7d02 7c02 4400  ..}.|.....}.|.D.
-00002410: 5d5e 7d03 7c00 a005 7406 7407 7408 7c03  ]^}.|...t.t.t.|.
-00002420: a104 7d04 7409 7c04 8301 7d05 7c05 a00a  ..}.t.|...}.|...
-00002430: 7c01 6a0b a101 6401 1900 7d06 7c05 a00c  |.j...d...}.|...
-00002440: a100 4400 5d28 7d07 7c07 6402 6b02 725e  ..D.](}.|.d.k.r^
-00002450: 6403 7d07 7c00 a00d 740e 7c01 7c07 8302  d.}.|...t.|.|...
-00002460: 740e 7c06 7c07 8302 a102 0100 714e 711a  t.|.|.......qNq.
-00002470: 6400 5300 2904 4e72 0100 0000 7256 0000  d.S.).Nr....rV..
-00002480: 00da 0b63 6f6f 7264 696e 6174 6573 290f  ...coordinates).
-00002490: 7215 0000 00da 076f 626a 6563 7473 da03  r......objects..
-000024a0: 616c 6cda 0566 6972 7374 721b 0000 0072  all..firstr....r
-000024b0: 1d00 0000 7209 0000 0072 1c00 0000 720d  ....r....r....r.
-000024c0: 0000 0072 0600 0000 5a13 6765 745f 6461  ...r....Z.get_da
-000024d0: 7461 7365 745f 636f 6e74 656e 7472 5000  taset_contentrP.
-000024e0: 0000 7257 0000 0072 1e00 0000 da07 6765  ..rW...r......ge
-000024f0: 7461 7474 7229 0872 2700 0000 da06 6761  tattr).r'.....ga
-00002500: 7264 656e 722a 0000 0072 2b00 0000 721f  rdenr*...r+...r.
-00002510: 0000 0072 2d00 0000 5a07 6761 7264 656e  ...r-...Z.garden
-00002520: 5fda 0a66 6965 6c64 5f6e 616d 6572 2e00  _..field_namer..
-00002530: 0000 722e 0000 0072 2f00 0000 da18 7465  ..r....r/.....te
-00002540: 7374 5f67 6574 5f64 6174 6173 6574 5f63  st_get_dataset_c
-00002550: 6f6e 7465 6e74 c001 0000 7314 0000 0000  ontent....s.....
-00002560: 020e 0208 0108 0210 0108 0210 020c 0208  ................
-00002570: 0104 027a 2954 6573 744d 6170 436c 7573  ...z)TestMapClus
-00002580: 7465 7265 722e 7465 7374 5f67 6574 5f64  terer.test_get_d
-00002590: 6174 6173 6574 5f63 6f6e 7465 6e74 6301  ataset_contentc.
-000025a0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-000025b0: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
-000025c0: 723a 0000 0072 2e00 0000 a901 7227 0000  r:...r......r'..
-000025d0: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-000025e0: da13 7465 7374 5f70 616e 6e65 645f 7265  ..test_panned_re
-000025f0: 7175 6573 74d3 0100 0073 0200 0000 0001  quest....s......
-00002600: 7a24 5465 7374 4d61 7043 6c75 7374 6572  z$TestMapCluster
-00002610: 6572 2e74 6573 745f 7061 6e6e 6564 5f72  er.test_panned_r
-00002620: 6571 7565 7374 6301 0000 0000 0000 0000  equestc.........
-00002630: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00002640: 0400 0000 6400 5300 723a 0000 0072 2e00  ....d.S.r:...r..
-00002650: 0000 7275 0000 0072 2e00 0000 722e 0000  ..ru...r....r...
-00002660: 0072 2f00 0000 da17 7465 7374 5f7a 6f6f  .r/.....test_zoo
-00002670: 6d5f 6c65 7665 6c5f 6368 616e 6765 64d6  m_level_changed.
-00002680: 0100 0073 0200 0000 0001 7a28 5465 7374  ...s......z(Test
-00002690: 4d61 7043 6c75 7374 6572 6572 2e74 6573  MapClusterer.tes
-000026a0: 745f 7a6f 6f6d 5f6c 6576 656c 5f63 6861  t_zoom_level_cha
-000026b0: 6e67 6564 6301 0000 0000 0000 0000 0000  ngedc...........
-000026c0: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-000026d0: 0000 6400 5300 723a 0000 0072 2e00 0000  ..d.S.r:...r....
-000026e0: 7275 0000 0072 2e00 0000 722e 0000 0072  ru...r....r....r
-000026f0: 2f00 0000 da18 7465 7374 5f63 6c75 7374  /.....test_clust
-00002700: 6572 7479 7065 5f63 6861 6e67 6564 d901  ertype_changed..
-00002710: 0000 7302 0000 0000 017a 2954 6573 744d  ..s......z)TestM
-00002720: 6170 436c 7573 7465 7265 722e 7465 7374  apClusterer.test
-00002730: 5f63 6c75 7374 6572 7479 7065 5f63 6861  _clustertype_cha
-00002740: 6e67 6564 6301 0000 0000 0000 0000 0000  ngedc...........
-00002750: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-00002760: 0000 6400 5300 723a 0000 0072 2e00 0000  ..d.S.r:...r....
-00002770: 7275 0000 0072 2e00 0000 722e 0000 0072  ru...r....r....r
-00002780: 2f00 0000 da10 7465 7374 5f63 6c65 6172  /.....test_clear
-00002790: 5f63 6163 6865 dc01 0000 7302 0000 0000  _cache....s.....
-000027a0: 017a 2154 6573 744d 6170 436c 7573 7465  .z!TestMapCluste
-000027b0: 7265 722e 7465 7374 5f63 6c65 6172 5f63  rer.test_clear_c
-000027c0: 6163 6865 4e29 19da 085f 5f6e 616d 655f  acheN)...__name_
-000027d0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000027e0: 5f71 7561 6c6e 616d 655f 5f72 3000 0000  _qualname__r0...
-000027f0: 7232 0000 0072 3900 0000 723c 0000 0072  r2...r9...r<...r
-00002800: 3d00 0000 7240 0000 0072 4800 0000 724c  =...r@...rH...rL
-00002810: 0000 0072 4d00 0000 724f 0000 0072 5900  ...rM...rO...rY.
-00002820: 0000 725a 0000 0072 6200 0000 7264 0000  ..rZ...rb...rd..
-00002830: 0072 6500 0000 726b 0000 0072 6c00 0000  .re...rk...rl...
-00002840: 7274 0000 0072 7600 0000 7277 0000 0072  rt...rv...rw...r
-00002850: 7800 0000 7279 0000 0072 2e00 0000 722e  x...ry...r....r.
-00002860: 0000 0072 2e00 0000 722f 0000 0072 1800  ...r....r/...r..
-00002870: 0000 1400 0000 732c 0000 0008 0308 1608  ......s,........
-00002880: 1208 2208 1608 1308 1708 2508 1708 1508  ..".......%.....
-00002890: 1308 1608 1508 2608 1708 1808 1b08 2008  ......&....... .
-000028a0: 1308 0308 0308 0372 1800 0000 6300 0000  .......r....c...
-000028b0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-000028c0: 0040 0000 0073 3400 0000 6500 5a01 6400  .@...s4...e.Z.d.
-000028d0: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
-000028e0: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
-000028f0: 5a06 6409 640a 8400 5a07 640b 5300 290c  Z.d.d...Z.d.S.).
-00002900: da1d 5465 7374 4d61 7043 6c75 7374 6572  ..TestMapCluster
-00002910: 6572 436f 6e74 656e 7443 6f75 6e74 7363  erContentCountsc
-00002920: 0100 0000 0000 0000 0000 0000 0d00 0000  ................
-00002930: 0a00 0000 4300 0000 736e 0100 0064 017d  ....C...sn...d.}
-00002940: 0164 0264 0364 0464 059c 0367 017d 0264  .d.d.d.d...g.}.d
-00002950: 0664 0764 0864 0464 059c 0367 0169 0164  .d.d.d.d...g.i.d
-00002960: 0664 0764 0864 0964 059c 0367 0169 0164  .d.d.d.d...g.i.d
-00002970: 0a9c 027d 0374 0044 0090 015d 2a7d 0474  ...}.t.D...]*}.t
-00002980: 0144 0090 015d 1e7d 0574 0274 0374 0474  .D...].}.t.t.t.t
-00002990: 0566 0444 0090 015d 0a7d 067c 0474 066b  .f.D...].}.|.t.k
-000029a0: 0272 707c 0574 076b 0372 7071 587c 0574  .rp|.t.k.rpqX|.t
-000029b0: 076b 0272 827c 0674 036b 0372 8271 587c  .k.r.|.t.k.r.qX|
-000029c0: 00a0 087c 057c 017c 047c 02a1 047d 0774  ...|.|.|.|...}.t
-000029d0: 097c 0774 0a64 0b8d 027d 087c 08a0 0b7c  .|.t.d...}.|...|
-000029e0: 067c 057c 027c 017c 03a1 057d 0964 0c64  .|.|.|.|...}.d.d
-000029f0: 0d64 0c69 0164 0d64 0c69 0164 0a9c 0264  .d.i.d.d.i.d...d
-00002a00: 0e9c 027d 0a7c 00a0 0c7c 097c 0aa1 0201  ...}.|...|.|....
-00002a10: 007c 0574 076b 0290 0172 2c7c 00a0 0d64  .|.t.k...r,|...d
-00002a20: 0f64 03a1 0201 007c 00a0 0d64 1064 11a1  .d.....|...d.d..
-00002a30: 0201 007c 08a0 0b7c 067c 057c 027c 017c  ...|...|.|.|.|.|
-00002a40: 03a1 057d 0964 1264 0d64 0c69 0164 0d64  ...}.d.d.d.i.d.d
-00002a50: 1269 0164 0a9c 0264 0e9c 027d 0a7c 00a0  .i.d...d...}.|..
-00002a60: 0c7c 097c 0aa1 0201 0074 0e6a 0fa0 10a1  .|.|.....t.j....
-00002a70: 007d 0b7c 0b44 005d 0e7d 0c7c 0ca0 11a1  .}.|.D.].}.|....
-00002a80: 0001 0090 0171 3a74 0e6a 0fa0 10a1 007d  .....q:t.j.....}
-00002a90: 0b7c 00a0 0c7c 0ba0 12a1 0064 0ca1 0201  .|...|.....d....
-00002aa0: 0071 5871 4671 3c64 0053 0029 134e 7266  .qXqFq<d.S.).Nrf
-00002ab0: 0000 0072 5200 0000 da05 7374 6f6e 65fa  ...rR.....stone.
-00002ac0: 013d a903 da06 636f 6c75 6d6e da05 7661  .=....column..va
-00002ad0: 6c75 65da 086f 7065 7261 746f 7272 2b00  lue..operatorr+.
-00002ae0: 0000 7254 0000 0054 7a02 213d 2902 da04  ..rT...Tz.!=)...
-00002af0: 6672 6565 5a04 7061 6964 a901 7222 0000  freeZ.paid..r"..
-00002b00: 0072 0100 0000 725f 0000 0029 0272 5f00  .r....r_...).r_.
-00002b10: 0000 da0b 6d6f 6475 6c61 7469 6f6e 73fa  ....modulations.
-00002b20: 066e 616d 6520 31fa 066e 616d 6520 32da  .name 1..name 2.
-00002b30: 0666 6c6f 7765 7272 3100 0000 2913 7208  .flowerr1...).r.
-00002b40: 0000 0072 0b00 0000 720e 0000 0072 0f00  ...r....r....r..
-00002b50: 0000 7210 0000 0072 1100 0000 720d 0000  ..r....r....r...
-00002b60: 0072 0900 0000 721d 0000 0072 0600 0000  .r....r....r....
-00002b70: da0e 5445 5354 5f47 5249 445f 5349 5a45  ..TEST_GRID_SIZE
-00002b80: 5a16 6765 745f 6d61 705f 636f 6e74 656e  Z.get_map_conten
-00002b90: 745f 636f 756e 7473 721e 0000 00da 0c63  t_countsr......c
-00002ba0: 7265 6174 655f 706f 696e 7472 1500 0000  reate_pointr....
-00002bb0: 726e 0000 0072 6f00 0000 da06 6465 6c65  rn...ro.....dele
-00002bc0: 7465 725f 0000 0029 0d72 2700 0000 722c  ter_...).r'...r,
-00002bd0: 0000 0072 2b00 0000 7286 0000 0072 2800  ...r+...r....r(.
-00002be0: 0000 7229 0000 0072 3600 0000 721f 0000  ..r)...r6...r...
-00002bf0: 0072 2d00 0000 da06 7265 7375 6c74 da0f  .r-.....result..
-00002c00: 6578 7065 6374 6564 5f72 6573 756c 74da  expected_result.
-00002c10: 0767 6172 6465 6e73 7272 0000 0072 2e00  .gardensrr...r..
-00002c20: 0000 722e 0000 0072 2f00 0000 da1a 7465  ..r....r/.....te
-00002c30: 7374 5f67 6574 5f6d 6170 5f63 6f6e 7465  st_get_map_conte
-00002c40: 6e74 5f63 6f75 6e74 e201 0000 7378 0000  nt_count....sx..
-00002c50: 0000 0204 0502 0102 0102 fd04 ff04 0b02  ................
-00002c60: 0202 0102 0102 fd04 ff02 fe02 0b02 0202  ................
-00002c70: 0102 0102 fd04 ff02 ff02 f506 170a 010a  ................
-00002c80: 0212 0210 0102 0210 0102 0210 010c 0212  ................
-00002c90: 0302 0302 0002 ff02 0402 0002 ff02 fc04  ................
-00002ca0: fe06 0b0c 020a 020c 010c 0212 0302 0302  ................
-00002cb0: 0002 ff02 0402 0002 ff02 fc04 fe06 0e0c  ................
-00002cc0: 020a 0108 010c 030a 027a 3854 6573 744d  .........z8TestM
-00002cd0: 6170 436c 7573 7465 7265 7243 6f6e 7465  apClustererConte
-00002ce0: 6e74 436f 756e 7473 2e74 6573 745f 6765  ntCounts.test_ge
-00002cf0: 745f 6d61 705f 636f 6e74 656e 745f 636f  t_map_content_co
-00002d00: 756e 7463 0100 0000 0000 0000 0000 0000  untc............
-00002d10: 0c00 0000 0600 0000 4300 0000 7332 0100  ........C...s2..
-00002d20: 0064 017d 0174 007d 0274 017d 0367 007d  .d.}.t.}.t.}.g.}
-00002d30: 047c 00a0 027c 027c 017c 037c 04a1 047d  .|...|.|.|.|...}
-00002d40: 0574 037c 0574 0464 028d 027d 0674 057d  .t.|.t.d...}.t.}
-00002d50: 077c 06a0 067c 077c 027c 01a1 037d 087c  .|...|.|.|...}.|
-00002d60: 06a0 077c 087c 04a1 027d 097c 00a0 087c  ...|.|...}.|...|
-00002d70: 0964 03a1 0201 007c 00a0 0964 0464 05a1  .d.....|...d.d..
-00002d80: 0201 007c 06a0 077c 087c 04a1 027d 097c  ...|...|.|...}.|
-00002d90: 00a0 087c 0964 06a1 0201 007c 00a0 0964  ...|.d.....|...d
-00002da0: 0764 08a1 0201 007c 06a0 077c 087c 04a1  .d.....|...|.|..
-00002db0: 027d 097c 00a0 087c 0964 09a1 0201 0064  .}.|...|.d.....d
-00002dc0: 0a64 0564 0b64 0c9c 0367 017d 047c 06a0  .d.d.d...g.}.|..
-00002dd0: 077c 087c 04a1 027d 097c 00a0 087c 0964  .|.|...}.|...|.d
-00002de0: 06a1 0201 0064 0a64 0564 0b64 0c9c 0364  .....d.d.d.d...d
-00002df0: 0a64 0864 0b64 0d64 0e9c 0467 027d 047c  .d.d.d.d...g.}.|
-00002e00: 06a0 077c 087c 04a1 027d 097c 00a0 087c  ...|.|...}.|...|
-00002e10: 0964 09a1 0201 0074 0a6a 0ba0 0ca1 007d  .d.....t.j.....}
-00002e20: 0a7c 0a44 005d 0e7d 0b7c 0ba0 0da1 0001  .|.D.].}.|......
-00002e30: 0090 0171 0474 0a6a 0ba0 0ca1 007d 0a7c  ...q.t.j.....}.|
-00002e40: 00a0 087c 0aa0 0ea1 0064 03a1 0201 0064  ...|.....d.....d
-00002e50: 0053 0029 0f4e 7266 0000 0072 8500 0000  .S.).Nrf...r....
-00002e60: 7201 0000 0072 8700 0000 727e 0000 0072  r....r....r~...r
-00002e70: 3100 0000 7288 0000 0072 8900 0000 7233  1...r....r....r3
-00002e80: 0000 0072 5200 0000 727f 0000 0072 8000  ...rR...r....r..
-00002e90: 0000 da02 4f52 2904 7281 0000 0072 8200  ....OR).r....r..
-00002ea0: 0000 7283 0000 00da 0f6c 6f67 6963 616c  ..r......logical
-00002eb0: 4f70 6572 6174 6f72 290f 7209 0000 0072  Operator).r....r
-00002ec0: 0c00 0000 721d 0000 0072 0600 0000 728a  ....r....r....r.
-00002ed0: 0000 0072 0f00 0000 da1b 6765 745f 6765  ...r......get_ge
-00002ee0: 6f6d 6574 7269 6573 5f66 6f72 5f63 6f75  ometries_for_cou
-00002ef0: 6e74 696e 675a 1771 7565 7279 5f6d 6170  ntingZ.query_map
-00002f00: 5f63 6f6e 7465 6e74 5f63 6f75 6e74 721e  _content_countr.
-00002f10: 0000 0072 8b00 0000 7215 0000 0072 6e00  ...r....r....rn.
-00002f20: 0000 726f 0000 0072 8c00 0000 725f 0000  ..ro...r....r_..
-00002f30: 0029 0c72 2700 0000 722c 0000 0072 2900  .).r'...r,...r).
-00002f40: 0000 7228 0000 0072 2b00 0000 721f 0000  ..r(...r+...r...
-00002f50: 0072 2d00 0000 7236 0000 005a 1767 656f  .r-...r6...Z.geo
-00002f60: 6d65 7472 6965 735f 666f 725f 636f 756e  metries_for_coun
-00002f70: 7469 6e67 725f 0000 0072 8f00 0000 7272  tingr_...r....rr
-00002f80: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00002f90: 0000 da1c 7465 7374 5f71 7565 7279 5f6d  ....test_query_m
-00002fa0: 6170 5f63 6f6e 7465 6e74 5f63 6f75 6e74  ap_content_count
-00002fb0: 4402 0000 7350 0000 0000 0204 0104 0104  D...sP..........
-00002fc0: 0304 0210 010c 0204 020e 020c 010c 020c  ................
-00002fd0: 020c 010c 020c 020c 010c 0502 0102 0102  ................
-00002fe0: fd04 ff04 080c 010c 0402 0102 0102 fd04  ................
-00002ff0: 0602 0102 0102 0102 fc04 fa04 0e0c 010c  ................
-00003000: 020a 0108 010c 030a 027a 3a54 6573 744d  .........z:TestM
-00003010: 6170 436c 7573 7465 7265 7243 6f6e 7465  apClustererConte
-00003020: 6e74 436f 756e 7473 2e74 6573 745f 7175  ntCounts.test_qu
-00003030: 6572 795f 6d61 705f 636f 6e74 656e 745f  ery_map_content_
-00003040: 636f 756e 7463 0100 0000 0000 0000 0000  countc..........
-00003050: 0000 0a00 0000 0900 0000 4300 0000 73aa  ..........C...s.
-00003060: 0000 0064 017d 0174 0044 005d 9c7d 0274  ...d.}.t.D.].}.t
-00003070: 0144 005d 927d 0374 0274 0374 0474 0566  .D.].}.t.t.t.t.f
-00003080: 0444 005d 807d 047c 0274 066b 0272 367c  .D.].}.|.t.k.r6|
-00003090: 0374 076b 0372 3671 207c 0374 076b 0272  .t.k.r6q |.t.k.r
-000030a0: 487c 0474 036b 0372 4871 2067 007d 057c  H|.t.k.rHq g.}.|
-000030b0: 00a0 087c 037c 017c 027c 05a1 047d 0674  ...|.|.|.|...}.t
-000030c0: 097c 0674 0a64 028d 027d 077c 07a0 0b7c  .|.t.d...}.|...|
-000030d0: 047c 037c 01a1 037d 087c 00a0 0c74 0d7c  .|.|...}.|...t.|
-000030e0: 0874 0e83 02a1 0101 007c 0844 005d 147d  .t.......|.D.].}
-000030f0: 097c 00a0 0c64 037c 096a 0f6b 06a1 0101  .|...d.|.j.k....
-00003100: 0071 8a71 2071 1071 0864 0053 0029 044e  .q.q q.q.d.S.).N
-00003110: 7266 0000 0072 8500 0000 da07 504f 4c59  rf...r......POLY
-00003120: 474f 4e29 1072 0800 0000 720b 0000 0072  GON).r....r....r
-00003130: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
-00003140: 0000 0072 0d00 0000 7209 0000 0072 1d00  ...r....r....r..
-00003150: 0000 7206 0000 0072 8a00 0000 7293 0000  ..r....r....r...
-00003160: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
-00003170: da03 776b 7429 0a72 2700 0000 722c 0000  ..wkt).r'...r,..
-00003180: 0072 2800 0000 7229 0000 0072 3600 0000  .r(...r)...r6...
-00003190: 722b 0000 0072 1f00 0000 722d 0000 0072  r+...r....r-...r
-000031a0: 3700 0000 7241 0000 0072 2e00 0000 722e  7...rA...r....r.
-000031b0: 0000 0072 2f00 0000 da20 7465 7374 5f67  ...r/.... test_g
-000031c0: 6574 5f67 656f 6d65 7472 6965 735f 666f  et_geometries_fo
-000031d0: 725f 636f 756e 7469 6e67 8802 0000 731e  r_counting....s.
-000031e0: 0000 0000 0204 0208 0108 0210 0210 0102  ................
-000031f0: 0210 0102 0204 0210 010c 020e 0210 0208  ................
-00003200: 027a 3e54 6573 744d 6170 436c 7573 7465  .z>TestMapCluste
-00003210: 7265 7243 6f6e 7465 6e74 436f 756e 7473  rerContentCounts
-00003220: 2e74 6573 745f 6765 745f 6765 6f6d 6574  .test_get_geomet
-00003230: 7269 6573 5f66 6f72 5f63 6f75 6e74 696e  ries_for_countin
-00003240: 6763 0100 0000 0000 0000 0000 0000 0a00  gc..............
-00003250: 0000 0800 0000 4300 0000 738e 0000 0067  ......C...s....g
-00003260: 007d 0164 017d 0274 0044 005d 7c7d 0374  .}.d.}.t.D.]|}.t
-00003270: 0144 005d 727d 047c 00a0 027c 047c 027c  .D.]r}.|...|.|.|
-00003280: 037c 01a1 047d 0574 037c 0574 0464 028d  .|...}.t.|.t.d..
-00003290: 027d 067c 06a0 0574 06a1 017d 077c 06a0  .}.|...t...}.|..
-000032a0: 077c 077c 02a1 027d 087c 00a0 0874 097c  .|.|...}.|...t.|
-000032b0: 0883 0164 03a1 0201 007c 00a0 087c 086a  ...d.....|...|.j
-000032c0: 0a64 04a1 0201 007c 08a0 0b64 05a1 0101  .d.....|...d....
-000032d0: 0064 067d 097c 00a0 087c 0974 097c 0883  .d.}.|...|.t.|..
-000032e0: 01a1 0201 0071 1471 0c64 0053 0029 074e  .....q.q.d.S.).N
-000032f0: 7266 0000 0072 8500 0000 7aa7 5352 4944  rf...r....z.SRID
-00003300: 3d33 3835 373b 504f 4c59 474f 4e20 2828  =3857;POLYGON ((
-00003310: 3937 3833 3933 2e39 3632 3035 2035 3934  978393.96205 594
-00003320: 3836 3335 2e32 3839 3031 362c 2031 3536  8635.289016, 156
-00003330: 3534 3330 2e33 3339 3238 2035 3934 3836  5430.33928 59486
-00003340: 3335 2e32 3839 3031 362c 2031 3536 3534  35.289016, 15654
-00003350: 3330 2e33 3339 3238 2036 3537 3438 3037  30.33928 6574807
-00003360: 2e34 3234 3732 382c 2039 3738 3339 332e  .424728, 978393.
-00003370: 3936 3230 3520 3635 3734 3830 372e 3432  96205 6574807.42
-00003380: 3437 3238 2c20 3937 3833 3933 2e39 3632  4728, 978393.962
-00003390: 3035 2035 3934 3836 3335 2e32 3839 3031  05 5948635.28901
-000033a0: 3629 2972 1a00 0000 7242 0000 007a c553  6))r....rB...z.S
-000033b0: 5249 443d 3433 3236 3b50 4f4c 5947 4f4e  RID=4326;POLYGON
-000033c0: 2028 2838 2e37 3839 3036 3234 3939 3939   ((8.78906249999
-000033d0: 3737 2034 372e 3034 3031 3832 3134 3332  77 47.0401821432
-000033e0: 3738 3839 2c20 3134 2e30 3632 3439 3939  7889, 14.0624999
-000033f0: 3939 3939 3633 3220 3437 2e30 3430 3138  9999632 47.04018
-00003400: 3231 3433 3237 3838 392c 2031 342e 3036  214327889, 14.06
-00003410: 3234 3939 3939 3939 3936 3332 2035 302e  249999999632 50.
-00003420: 3733 3634 3535 3133 3535 3930 392c 2038  7364551355909, 8
-00003430: 2e37 3839 3036 3234 3939 3939 3737 2035  .7890624999977 5
-00003440: 302e 3733 3634 3535 3133 3535 3930 392c  0.7364551355909,
-00003450: 2038 2e37 3839 3036 3234 3939 3939 3737   8.7890624999977
-00003460: 2034 372e 3034 3031 3832 3134 3332 3738   47.040182143278
-00003470: 3839 2929 290c 7208 0000 0072 0b00 0000  89))).r....r....
-00003480: 721d 0000 0072 0600 0000 728a 0000 0072  r....r....r....r
-00003490: 3b00 0000 720f 0000 005a 1573 6e61 705f  ;...r....Z.snap_
-000034a0: 7669 6577 706f 7274 5f74 6f5f 6772 6964  viewport_to_grid
-000034b0: 721e 0000 00da 0373 7472 7235 0000 0072  r......strr5...r
-000034c0: 4600 0000 290a 7227 0000 0072 2b00 0000  F...).r'...r+...
-000034d0: 722c 0000 0072 2800 0000 7229 0000 0072  r,...r(...r)...r
-000034e0: 1f00 0000 722d 0000 0072 3700 0000 5a0e  ....r-...r7...Z.
-000034f0: 6772 6964 5f72 6563 7461 6e67 6c65 5a0c  grid_rectangleZ.
-00003500: 706f 6c79 676f 6e5f 3433 3236 722e 0000  polygon_4326r...
-00003510: 0072 2e00 0000 722f 0000 00da 1a74 6573  .r....r/.....tes
-00003520: 745f 736e 6170 5f76 6965 7770 6f72 745f  t_snap_viewport_
-00003530: 746f 5f67 7269 64a5 0200 0073 1a00 0000  to_grid....s....
-00003540: 0002 0401 0402 0801 0802 1002 0c03 0a02  ................
-00003550: 0c02 1001 0e02 0a02 0402 7a38 5465 7374  ..........z8Test
-00003560: 4d61 7043 6c75 7374 6572 6572 436f 6e74  MapClustererCont
-00003570: 656e 7443 6f75 6e74 732e 7465 7374 5f73  entCounts.test_s
+000000c0: 6d1c 5a1c 6d1d 5a1d 6d1e 5a1e 0100 6400  m.Z.m.Z.m.Z...d.
+000000d0: 640a 6c1f 6d20 5a20 0100 6400 640b 6c21  d.l.m Z ..d.d.l!
+000000e0: 5a21 640c 5a22 640d 5a23 4700 640e 640f  Z!d.Z"d.Z#G.d.d.
+000000f0: 8400 640f 651d 651c 6501 8305 5a24 4700  ..d.e.e.e...Z$G.
+00000100: 6410 6411 8400 6411 651d 651e 6501 8305  d.d...d.e.e.e...
+00000110: 5a25 6502 6412 6413 6702 6414 8d01 4700  Z%e.d.d.g.d...G.
+00000120: 6415 6416 8400 6416 651d 651c 6501 8305  d.d...d.e.e.e...
+00000130: 8301 5a26 640b 5300 2917 e900 0000 0029  ..Z&d.S.)......)
+00000140: 03da 0854 6573 7443 6173 65da 116f 7665  ...TestCase..ove
+00000150: 7272 6964 655f 7365 7474 696e 6773 da0f  rride_settings..
+00000160: 6d6f 6469 6679 5f73 6574 7469 6e67 7329  modify_settings)
+00000170: 01da 0873 6574 7469 6e67 7329 01da 0c47  ...settings)...G
+00000180: 454f 5347 656f 6d65 7472 7929 02da 1053  EOSGeometry)...S
+00000190: 7061 7469 616c 5265 6665 7265 6e63 65da  patialReference.
+000001a0: 0e43 6f6f 7264 5472 616e 7366 6f72 6d29  .CoordTransform)
+000001b0: 01da 0c4d 6170 436c 7573 7465 7265 7229  ...MapClusterer)
+000001c0: 01da 084d 6170 546f 6f6c 7329 06da 0d43  ...MapTools)...C
+000001d0: 4c55 5354 4552 5f54 5950 4553 da16 4745  LUSTER_TYPES..GE
+000001e0: 4f4d 4554 5259 5f54 5950 455f 5649 4557  OMETRY_TYPE_VIEW
+000001f0: 504f 5254 da12 4745 4f4d 4554 5259 5f54  PORT..GEOMETRY_T
+00000200: 5950 455f 4152 4541 da0e 4745 4f4d 4554  YPE_AREA..GEOMET
+00000210: 5259 5f54 5950 4553 da13 434c 5553 5445  RY_TYPES..CLUSTE
+00000220: 525f 5459 5045 5f4b 4d45 414e 53da 1143  R_TYPE_KMEANS..C
+00000230: 4c55 5354 4552 5f54 5950 455f 4752 4944  LUSTER_TYPE_GRID
+00000240: 2904 da0f 4745 4f4a 534f 4e5f 504f 4c59  )...GEOJSON_POLY
+00000250: 474f 4eda 1147 454f 4a53 4f4e 5f52 4543  GON..GEOJSON_REC
+00000260: 5441 4e47 4c45 da14 4745 4f4a 534f 4e5f  TANGLE..GEOJSON_
+00000270: 4d55 4c54 4950 4f4c 5947 4f4e da19 4745  MULTIPOLYGON..GE
+00000280: 4f4a 534f 4e5f 4645 4154 5552 4543 4f4c  OJSON_FEATURECOL
+00000290: 4c45 4354 494f 4e29 03da 0757 6974 6847  LECTION)...WithG
+000002a0: 4953 da0b 5769 7468 4669 6c74 6572 73da  IS..WithFilters.
+000002b0: 0b57 6974 6847 6172 6465 6e73 2901 da07  .WithGardens)...
+000002c0: 4761 7264 656e 734e e907 0000 00e9 0001  GardensN........
+000002d0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000002e0: 0000 0002 0000 0040 0000 0073 bc00 0000  .......@...s....
+000002f0: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
+00000300: 6403 6404 8400 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
+00000310: 6407 6408 8400 5a06 6409 640a 8400 5a07  d.d...Z.d.d...Z.
+00000320: 640b 640c 8400 5a08 640d 640e 8400 5a09  d.d...Z.d.d...Z.
+00000330: 640f 6410 8400 5a0a 6411 6412 8400 5a0b  d.d...Z.d.d...Z.
+00000340: 6413 6414 8400 5a0c 6415 6416 8400 5a0d  d.d...Z.d.d...Z.
+00000350: 6417 6418 8400 5a0e 6419 641a 8400 5a0f  d.d...Z.d.d...Z.
+00000360: 641b 641c 8400 5a10 641d 641e 8400 5a11  d.d...Z.d.d...Z.
+00000370: 641f 6420 8400 5a12 6421 6422 8400 5a13  d.d ..Z.d!d"..Z.
+00000380: 6423 6424 8400 5a14 6425 6426 8400 5a15  d#d$..Z.d%d&..Z.
+00000390: 6427 6428 8400 5a16 6429 642a 8400 5a17  d'd(..Z.d)d*..Z.
+000003a0: 642b 642c 8400 5a18 642d 5300 292e da10  d+d,..Z.d-S.)...
+000003b0: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
+000003c0: 6301 0000 0000 0000 0000 0000 0008 0000  c...............
+000003d0: 0009 0000 0043 0000 0073 a000 0000 7400  .....C...s....t.
+000003e0: 4400 5d96 7d01 7401 4400 5d8c 7d02 7c00  D.].}.t.D.].}.|.
+000003f0: a002 a100 7d03 7c03 4400 5d7a 7d04 7403  ....}.|.D.]z}.t.
+00000400: 7d05 7c00 a004 7c02 7c05 7c01 7c04 a104  }.|...|.|.|.|...
+00000410: 7d06 7405 7c06 8301 7d07 7c00 a006 7c07  }.t.|...}.|...|.
+00000420: 6a07 7c06 a102 0100 7c00 a006 7c07 6a08  j.|.....|...|.j.
+00000430: 6401 a102 0100 7c00 a006 7c07 6a09 6402  d.....|...|.j.d.
+00000440: a102 0100 7c00 a006 7c07 6a0a 6403 a102  ....|...|.j.d...
+00000450: 0100 7c00 a006 7c07 6a0b 6a0c 740d a102  ..|...|.j.j.t...
+00000460: 0100 7c00 a00e 740f 7c07 6a10 7411 8302  ..|...t.|.j.t...
+00000470: a101 0100 711c 710c 7104 6400 5300 2904  ....q.q.q.d.S.).
+00000480: 4eda 0670 7562 6c69 63e9 110f 0000 721a  N..public.....r.
+00000490: 0000 0029 1272 0b00 0000 720e 0000 00da  ...).r....r.....
+000004a0: 1067 6574 5f74 6573 745f 6669 6c74 6572  .get_test_filter
+000004b0: 73da 0f54 4553 545f 5a4f 4f4d 5f4c 4556  s..TEST_ZOOM_LEV
+000004c0: 454c da11 6765 745f 636c 7573 7465 725f  EL..get_cluster_
+000004d0: 6361 6368 6572 0900 0000 da0b 6173 7365  cacher......asse
+000004e0: 7274 4571 7561 6cda 0d63 6c75 7374 6572  rtEqual..cluster
+000004f0: 5f63 6163 6865 da0b 7363 6865 6d61 5f6e  _cache..schema_n
+00000500: 616d 65da 0764 625f 7372 6964 da09 6772  ame..db_srid..gr
+00000510: 6964 5f73 697a 655a 086d 6170 746f 6f6c  id_sizeZ.maptool
+00000520: 73da 095f 5f63 6c61 7373 5f5f 720a 0000  s..__class__r...
+00000530: 00da 0a61 7373 6572 7454 7275 65da 0a69  ...assertTrue..i
+00000540: 7369 6e73 7461 6e63 655a 0f76 616c 6964  sinstanceZ.valid
+00000550: 5f6f 7065 7261 746f 7273 da04 6c69 7374  _operators..list
+00000560: 2908 da04 7365 6c66 da0b 636c 7573 7465  )...self..cluste
+00000570: 7274 7970 65da 0d67 656f 6d65 7472 795f  rtype..geometry_
+00000580: 7479 7065 da0c 6669 6c74 6572 5f6c 6973  type..filter_lis
+00000590: 7473 da07 6669 6c74 6572 73da 047a 6f6f  ts..filters..zoo
+000005a0: 6d72 2200 0000 da0d 6d61 705f 636c 7573  mr".....map_clus
+000005b0: 7465 7265 72a9 0072 3100 0000 fa46 2f68  terer..r1....F/h
+000005c0: 6f6d 652f 746f 6d2f 616e 7963 6c75 7374  ome/tom/anyclust
+000005d0: 6572 2f64 656d 6f2f 646a 616e 676f 2f61  er/demo/django/a
+000005e0: 6e79 636c 7573 7465 722f 7465 7374 732f  nycluster/tests/
+000005f0: 7465 7374 5f4d 6170 436c 7573 7465 7265  test_MapClustere
+00000600: 722e 7079 da09 7465 7374 5f69 6e69 7417  r.py..test_init.
+00000610: 0000 0073 1a00 0000 0002 0802 0802 0801  ...s............
+00000620: 0802 0401 1002 0802 0e01 0e01 0e01 0e01  ................
+00000630: 1001 7a1a 5465 7374 4d61 7043 6c75 7374  ..z.TestMapClust
+00000640: 6572 6572 2e74 6573 745f 696e 6974 6301  erer.test_initc.
+00000650: 0000 0000 0000 0000 0000 0009 0000 0009  ................
+00000660: 0000 0043 0000 0073 5a00 0000 7400 4400  ...C...sZ...t.D.
+00000670: 5d50 7d01 7401 4400 5d46 7d02 7c00 a002  ]P}.t.D.]F}.|...
+00000680: a100 7d03 7c03 4400 5d34 7d04 6401 7d05  ..}.|.D.]4}.d.}.
+00000690: 7c00 a003 7c02 7c05 7c01 7c04 a104 7d06  |...|.|.|.|...}.
+000006a0: 7404 7c06 8301 7d07 7c07 a005 a100 7d08  t.|...}.|.....}.
+000006b0: 7c00 a006 7c08 6402 a102 0100 711c 710c  |...|.d.....q.q.
+000006c0: 7104 6400 5300 2903 4ee9 0100 0000 721d  q.d.S.).N.....r.
+000006d0: 0000 0029 0772 0b00 0000 720e 0000 0072  ...).r....r....r
+000006e0: 1e00 0000 7220 0000 0072 0900 0000 5a11  ....r ...r....Z.
+000006f0: 6765 745f 6461 7461 6261 7365 5f73 7269  get_database_sri
+00000700: 6472 2100 0000 2909 722a 0000 0072 2b00  dr!...).r*...r+.
+00000710: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+00000720: 0072 2f00 0000 7222 0000 0072 3000 0000  .r/...r"...r0...
+00000730: 7224 0000 0072 3100 0000 7231 0000 0072  r$...r1...r1...r
+00000740: 3200 0000 da16 7465 7374 5f67 6574 5f64  2.....test_get_d
+00000750: 6174 6162 6173 655f 7372 6964 2d00 0000  atabase_srid-...
+00000760: 7312 0000 0000 0208 0208 0208 0108 0204  s...............
+00000770: 0110 0208 0208 017a 2754 6573 744d 6170  .......z'TestMap
+00000780: 436c 7573 7465 7265 722e 7465 7374 5f67  Clusterer.test_g
+00000790: 6574 5f64 6174 6162 6173 655f 7372 6964  et_database_srid
+000007a0: 6301 0000 0000 0000 0000 0000 000c 0000  c...............
+000007b0: 000a 0000 0043 0000 0073 d800 0000 7400  .....C...s....t.
+000007c0: 4400 5dce 7d01 7401 4400 5dc4 7d02 7c00  D.].}.t.D.].}.|.
+000007d0: a002 a100 7d03 7c03 4400 5db2 7d04 7403  ....}.|.D.].}.t.
+000007e0: 7d05 7c00 a004 7c02 7c05 7c01 7c04 a104  }.|...|.|.|.|...
+000007f0: 7d06 7405 7c06 8301 7d07 7406 7407 6602  }.t.|...}.t.t.f.
+00000800: 4400 5d46 7d08 7c07 a008 7c08 a101 7d09  D.]F}.|...|...}.
+00000810: 7c00 a009 740a 7c09 8301 6401 a102 0100  |...t.|...d.....
+00000820: 7c09 4400 5d22 7d0a 7c00 a00b 740c 7c0a  |.D.]"}.|...t.|.
+00000830: 740d 8302 a101 0100 7c00 a009 7c0a 6a0e  t.......|...|.j.
+00000840: 6402 a102 0100 7166 7144 7c07 a008 740f  d.....qfqD|...t.
+00000850: a101 7d0b 7c00 a009 740a 7c0b 8301 6403  ..}.|...t.|...d.
+00000860: a102 0100 7c0b 4400 5d22 7d0a 7c00 a00b  ....|.D.]"}.|...
+00000870: 740c 7c0a 740d 8302 a101 0100 7c00 a009  t.|.t.......|...
+00000880: 7c0a 6a0e 6402 a102 0100 71aa 711c 710c  |.j.d.....q.q.q.
+00000890: 7104 6400 5300 2904 4e72 3400 0000 721d  q.d.S.).Nr4...r.
+000008a0: 0000 00e9 0200 0000 2910 720b 0000 0072  ........).r....r
+000008b0: 0e00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+000008c0: 0000 0072 0900 0000 7211 0000 0072 1200  ...r....r....r..
+000008d0: 0000 5a1f 636f 6e76 6572 745f 6765 6f6a  ..Z.convert_geoj
+000008e0: 736f 6e5f 6665 6174 7572 655f 746f 5f67  son_feature_to_g
+000008f0: 656f 7372 2100 0000 da03 6c65 6e72 2700  eosr!.....lenr'.
+00000900: 0000 7228 0000 0072 0600 0000 da04 7372  ..r(...r......sr
+00000910: 6964 7213 0000 0029 0c72 2a00 0000 722b  idr....).r*...r+
+00000920: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
+00000930: 0000 722f 0000 0072 2200 0000 7230 0000  ..r/...r"...r0..
+00000940: 00da 0767 656f 6a73 6f6e da0f 6765 6f73  ...geojson..geos
+00000950: 5f67 656f 6d65 7472 6965 73da 0d67 656f  _geometries..geo
+00000960: 735f 6765 6f6d 6574 7279 5a12 6d70 5f67  s_geometryZ.mp_g
+00000970: 656f 735f 6765 6f6d 6574 7269 6573 7231  eos_geometriesr1
+00000980: 0000 0072 3100 0000 7232 0000 00da 2c74  ...r1...r2....,t
+00000990: 6573 745f 636f 6e76 6572 745f 6765 6f6a  est_convert_geoj
+000009a0: 736f 6e5f 6665 6174 7572 655f 746f 5f67  son_feature_to_g
+000009b0: 656f 735f 706f 6c79 676f 6e3f 0000 0073  eos_polygon?...s
+000009c0: 2c00 0000 0002 0801 0802 0801 0802 0401  ,...............
+000009d0: 1002 0802 0c02 0401 02ff 0403 1002 0801  ................
+000009e0: 1001 1202 0401 02ff 0403 1002 0801 1001  ................
+000009f0: 7a3d 5465 7374 4d61 7043 6c75 7374 6572  z=TestMapCluster
+00000a00: 6572 2e74 6573 745f 636f 6e76 6572 745f  er.test_convert_
+00000a10: 6765 6f6a 736f 6e5f 6665 6174 7572 655f  geojson_feature_
+00000a20: 746f 5f67 656f 735f 706f 6c79 676f 6e63  to_geos_polygonc
+00000a30: 0100 0000 0000 0000 0000 0000 0b00 0000  ................
+00000a40: 0a00 0000 4300 0000 737a 0000 0074 0044  ....C...sz...t.D
+00000a50: 005d 707d 0174 0144 005d 667d 027c 00a0  .]p}.t.D.]f}.|..
+00000a60: 02a1 007d 037c 0344 005d 547d 0474 037d  ...}.|.D.]T}.t.}
+00000a70: 057c 00a0 047c 027c 057c 017c 04a1 047d  .|...|.|.|.|...}
+00000a80: 0674 057c 0683 017d 0774 0674 0774 0866  .t.|...}.t.t.t.f
+00000a90: 0344 005d 287d 087c 07a0 097c 08a1 017d  .D.](}.|...|...}
+00000aa0: 097c 0944 005d 147d 0a7c 00a0 0a74 0b7c  .|.D.].}.|...t.|
+00000ab0: 0a74 0c83 02a1 0101 0071 5871 4671 1c71  .t.......qXqFq.q
+00000ac0: 0c71 0464 0053 00a9 014e 290d 720b 0000  .q.d.S...N).r...
+00000ad0: 0072 0e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000ae0: 7220 0000 0072 0900 0000 7211 0000 0072  r ...r....r....r
+00000af0: 1200 0000 7213 0000 00da 1763 6f6e 7665  ....r......conve
+00000b00: 7274 5f67 656f 6a73 6f6e 5f74 6f5f 6765  rt_geojson_to_ge
+00000b10: 6f73 7227 0000 0072 2800 0000 7206 0000  osr'...r(...r...
+00000b20: 0029 0b72 2a00 0000 722b 0000 0072 2c00  .).r*...r+...r,.
+00000b30: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
+00000b40: 0072 2200 0000 7230 0000 0072 3900 0000  .r"...r0...r9...
+00000b50: 723a 0000 0072 3b00 0000 7231 0000 0072  r:...r;...r1...r
+00000b60: 3100 0000 7232 0000 00da 2474 6573 745f  1...r2....$test_
+00000b70: 636f 6e76 6572 745f 6765 6f6a 736f 6e5f  convert_geojson_
+00000b80: 746f 5f67 656f 735f 6665 6174 7572 6561  to_geos_featurea
+00000b90: 0000 0073 1a00 0000 0002 0801 0802 0801  ...s............
+00000ba0: 0802 0401 1002 0802 0e02 0401 02ff 0403  ................
+00000bb0: 0801 7a35 5465 7374 4d61 7043 6c75 7374  ..z5TestMapClust
+00000bc0: 6572 6572 2e74 6573 745f 636f 6e76 6572  erer.test_conver
+00000bd0: 745f 6765 6f6a 736f 6e5f 746f 5f67 656f  t_geojson_to_geo
+00000be0: 735f 6665 6174 7572 6563 0100 0000 0000  s_featurec......
+00000bf0: 0000 0000 0000 0a00 0000 0900 0000 4300  ..............C.
+00000c00: 0000 736a 0000 0074 0044 005d 607d 0174  ..sj...t.D.]`}.t
+00000c10: 0144 005d 567d 027c 00a0 02a1 007d 037c  .D.]V}.|.....}.|
+00000c20: 0344 005d 447d 0474 037d 057c 00a0 047c  .D.]D}.t.}.|...|
+00000c30: 027c 057c 017c 04a1 047d 0674 057c 0683  .|.|.|...}.t.|..
+00000c40: 017d 077c 07a0 0674 07a1 017d 087c 0844  .}.|...t...}.|.D
+00000c50: 005d 147d 097c 00a0 0874 097c 0974 0a83  .].}.|...t.|.t..
+00000c60: 02a1 0101 0071 4a71 1c71 0c71 0464 0053  .....qJq.q.q.d.S
+00000c70: 0072 3d00 0000 290b 720b 0000 0072 0e00  .r=...).r....r..
+00000c80: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00000c90: 0072 0900 0000 723e 0000 0072 1400 0000  .r....r>...r....
+00000ca0: 7227 0000 0072 2800 0000 7206 0000 0029  r'...r(...r....)
+00000cb0: 0a72 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
+00000cc0: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
+00000cd0: 2200 0000 7230 0000 0072 3a00 0000 723b  "...r0...r:...r;
+00000ce0: 0000 0072 3100 0000 7231 0000 0072 3200  ...r1...r1...r2.
+00000cf0: 0000 da2e 7465 7374 5f63 6f6e 7665 7274  ....test_convert
+00000d00: 5f67 656f 6a73 6f6e 5f74 6f5f 6765 6f73  _geojson_to_geos
+00000d10: 5f66 6561 7475 7265 636f 6c6c 6563 7469  _featurecollecti
+00000d20: 6f6e 7700 0000 7318 0000 0000 0208 0108  onw...s.........
+00000d30: 0208 0108 0204 0110 0208 0104 0102 ff04  ................
+00000d40: 0308 017a 3f54 6573 744d 6170 436c 7573  ...z?TestMapClus
+00000d50: 7465 7265 722e 7465 7374 5f63 6f6e 7665  terer.test_conve
+00000d60: 7274 5f67 656f 6a73 6f6e 5f74 6f5f 6765  rt_geojson_to_ge
+00000d70: 6f73 5f66 6561 7475 7265 636f 6c6c 6563  os_featurecollec
+00000d80: 7469 6f6e 6301 0000 0000 0000 0000 0000  tionc...........
+00000d90: 000b 0000 000a 0000 0043 0000 0073 7e00  .........C...s~.
+00000da0: 0000 7400 4400 5d74 7d01 7401 4400 5d6a  ..t.D.]t}.t.D.]j
+00000db0: 7d02 7c00 a002 a100 7d03 7c03 4400 5d58  }.|.....}.|.D.]X
+00000dc0: 7d04 7403 7d05 7c00 a004 7c02 7c05 7c01  }.t.}.|...|.|.|.
+00000dd0: 7c04 a104 7d06 7405 7c06 8301 7d07 7406  |...}.t.|...}.t.
+00000de0: 7407 7408 6603 4400 5d2c 7d08 7c07 a009  t.t.f.D.],}.|...
+00000df0: 7c08 7c02 7c05 a103 7d09 7c09 4400 5d14  |.|.|...}.|.D.].
+00000e00: 7d0a 7c00 a00a 740b 7c0a 740c 8302 a101  }.|...t.|.t.....
+00000e10: 0100 715c 7146 711c 710c 7104 6400 5300  ..q\qFq.q.q.d.S.
+00000e20: 723d 0000 0029 0d72 0b00 0000 720e 0000  r=...).r....r...
+00000e30: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000e40: 7209 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000e50: 1300 0000 da16 6765 745f 636c 7573 7465  ......get_cluste
+00000e60: 725f 6765 6f6d 6574 7269 6573 7227 0000  r_geometriesr'..
+00000e70: 0072 2800 0000 7206 0000 0029 0b72 2a00  .r(...r....).r*.
+00000e80: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+00000e90: 0072 2e00 0000 722f 0000 0072 2200 0000  .r....r/...r"...
+00000ea0: 7230 0000 0072 3900 0000 da12 636c 7573  r0...r9.....clus
+00000eb0: 7465 725f 6765 6f6d 6574 7269 6573 723b  ter_geometriesr;
+00000ec0: 0000 0072 3100 0000 7231 0000 0072 3200  ...r1...r1...r2.
+00000ed0: 0000 da24 7465 7374 5f67 6574 5f63 6c75  ...$test_get_clu
+00000ee0: 7374 6572 5f67 656f 6d65 7472 6965 735f  ster_geometries_
+00000ef0: 7669 6577 706f 7274 8a00 0000 731e 0000  viewport....s...
+00000f00: 0000 0208 0108 0308 0108 0204 0110 0208  ................
+00000f10: 020e 0204 0102 0002 0002 ff04 0308 017a  ...............z
+00000f20: 3554 6573 744d 6170 436c 7573 7465 7265  5TestMapClustere
+00000f30: 722e 7465 7374 5f67 6574 5f63 6c75 7374  r.test_get_clust
+00000f40: 6572 5f67 656f 6d65 7472 6965 735f 7669  er_geometries_vi
+00000f50: 6577 706f 7274 6301 0000 0000 0000 0000  ewportc.........
+00000f60: 0000 000d 0000 0009 0000 0043 0000 0073  ...........C...s
+00000f70: d600 0000 7400 4400 5dcc 7d01 7c00 a001  ....t.D.].}.|...
+00000f80: a100 7d02 7c02 4400 5dba 7d03 7402 7d04  ..}.|.D.].}.t.}.
+00000f90: 7c00 a003 7404 7c04 7c01 7c03 a104 7d05  |...t.|.|.|...}.
+00000fa0: 7405 7c05 8301 7d06 7406 7d07 7c06 a007  t.|...}.t.}.|...
+00000fb0: 7c07 7404 7c04 a103 7d08 7406 6401 1900  |.t.|...}.t.d...
+00000fc0: a008 a100 7d09 7409 740a a00b 7c09 a101  ....}.t.t...|...
+00000fd0: 6402 6403 8d02 7d0a 740c 740d 7c0a 6a0e  d.d...}.t.t.|.j.
+00000fe0: 8301 740d 6404 8301 8302 7d0b 7c0a a00f  ..t.d.....}.|...
+00000ff0: 7c0b a101 0100 7c00 a010 7c0a 6a11 7c08  |.....|...|.j.|.
+00001000: 6405 1900 6a11 a102 0100 7412 7406 7413  d...j.....t.t.t.
+00001010: 6603 4400 5d2c 7d07 7c06 a007 7c07 7404  f.D.],}.|...|.t.
+00001020: 7c04 a103 7d08 7c08 4400 5d14 7d0c 7c00  |...}.|.D.].}.|.
+00001030: a014 7415 7c0c 7409 8302 a101 0100 71b6  ..t.|.t.......q.
+00001040: 71a0 7114 7104 6400 5300 2906 4eda 0867  q.q.q.d.S.).N..g
+00001050: 656f 6d65 7472 79e9 e610 0000 2901 7238  eometry.....).r8
+00001060: 0000 0072 1d00 0000 7201 0000 0029 1672  ...r....r....).r
+00001070: 0b00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+00001080: 0000 0072 0d00 0000 7209 0000 0072 1200  ...r....r....r..
+00001090: 0000 7241 0000 00da 0463 6f70 7972 0600  ..rA.....copyr..
+000010a0: 0000 da04 6a73 6f6e da05 6475 6d70 7372  ....json..dumpsr
+000010b0: 0800 0000 7207 0000 0072 3800 0000 da09  ....r....r8.....
+000010c0: 7472 616e 7366 6f72 6d72 2100 0000 7239  transformr!...r9
+000010d0: 0000 0072 1100 0000 7213 0000 0072 2700  ...r....r....r'.
+000010e0: 0000 7228 0000 0029 0d72 2a00 0000 722b  ..r(...).r*...r+
+000010f0: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
+00001100: 0000 7222 0000 0072 3000 0000 7239 0000  ..r"...r0...r9..
+00001110: 0072 4200 0000 5a10 6d61 7463 6869 6e67  .rB...Z.matching
+00001120: 5f67 656f 6a73 6f6e 5a0c 696e 6974 6961  _geojsonZ.initia
+00001130: 6c5f 6765 6f73 da02 6374 723b 0000 0072  l_geos..ctr;...r
+00001140: 3100 0000 7231 0000 0072 3200 0000 da20  1...r1...r2.... 
+00001150: 7465 7374 5f67 6574 5f63 6c75 7374 6572  test_get_cluster
+00001160: 5f67 656f 6d65 7472 6965 735f 6172 6561  _geometries_area
+00001170: a100 0000 7344 0000 0000 0208 0308 0108  ....sD..........
+00001180: 0204 0110 0208 0204 0204 0102 0002 0002  ................
+00001190: ff04 030c 0102 0108 0002 ff06 0204 0104  ................
+000011a0: ff02 0106 ff04 020a 0208 0108 ff04 030e  ................
+000011b0: 0204 0102 0002 0002 ff04 0308 017a 3154  .............z1T
+000011c0: 6573 744d 6170 436c 7573 7465 7265 722e  estMapClusterer.
+000011d0: 7465 7374 5f67 6574 5f63 6c75 7374 6572  test_get_cluster
+000011e0: 5f67 656f 6d65 7472 6965 735f 6172 6561  _geometries_area
+000011f0: 6301 0000 0000 0000 0000 0000 0009 0000  c...............
+00001200: 0009 0000 0043 0000 0073 7a00 0000 7400  .....C...sz...t.
+00001210: 7d01 7401 4400 5d6c 7d02 7402 7403 7404  }.t.D.]l}.t.t.t.
+00001220: 6603 4400 5d5c 7d03 7c00 a005 a100 7d04  f.D.]\}.|.....}.
+00001230: 7c04 4400 5d4a 7d05 7c00 a006 7c02 7c01  |.D.]J}.|...|.|.
+00001240: 7407 7c05 a104 7d06 7408 7c06 8301 7d07  t.|...}.t.|...}.
+00001250: 6700 7d05 7c07 a009 7c03 7c02 7c01 7c05  g.}.|...|.|.|.|.
+00001260: a104 7d08 7c02 740a 6b02 7226 7c00 a00b  ..}.|.t.k.r&|...
+00001270: 740c 7c08 8301 6401 6b04 a101 0100 7126  t.|...d.k.....q&
+00001280: 7116 7108 6400 5300 a902 4e72 0100 0000  q.q.d.S...Nr....
+00001290: 290d 721f 0000 0072 0e00 0000 7211 0000  ).r....r....r...
+000012a0: 0072 1200 0000 7213 0000 0072 1e00 0000  .r....r....r....
+000012b0: 7220 0000 0072 0f00 0000 7209 0000 00da  r ...r....r.....
+000012c0: 0e6b 6d65 616e 735f 636c 7573 7465 7272  .kmeans_clusterr
+000012d0: 0c00 0000 7227 0000 0072 3700 0000 2909  ....r'...r7...).
+000012e0: 722a 0000 0072 2f00 0000 722c 0000 0072  r*...r/...r,...r
+000012f0: 3900 0000 722d 0000 0072 2e00 0000 7222  9...r-...r....r"
+00001300: 0000 0072 3000 0000 da07 6d61 726b 6572  ...r0.....marker
+00001310: 7372 3100 0000 7231 0000 0072 3200 0000  sr1...r1...r2...
+00001320: da13 7465 7374 5f6b 6d65 616e 735f 636c  ..test_kmeans_cl
+00001330: 7573 7465 72c6 0000 0073 1600 0000 0002  uster....s......
+00001340: 0402 0801 0e03 0801 0802 1002 0802 0402  ................
+00001350: 1002 0801 7a24 5465 7374 4d61 7043 6c75  ....z$TestMapClu
+00001360: 7374 6572 6572 2e74 6573 745f 6b6d 6561  sterer.test_kmea
+00001370: 6e73 5f63 6c75 7374 6572 6301 0000 0000  ns_clusterc.....
+00001380: 0000 0000 0000 000a 0000 0009 0000 0043  ...............C
+00001390: 0000 0073 6a00 0000 7400 7d01 7401 4400  ...sj...t.}.t.D.
+000013a0: 5d5c 7d02 7402 4400 5d52 7d03 7c00 a003  ]\}.t.D.]R}.|...
+000013b0: a100 7d04 7c04 4400 5d40 7d05 7c00 a004  ..}.|.D.]@}.|...
+000013c0: 7c03 7c01 7c02 7c05 a104 7d06 7405 7c06  |.|.|.|...}.t.|.
+000013d0: 8301 7d07 7406 7407 6602 4400 5d1a 7d08  ..}.t.t.f.D.].}.
+000013e0: 7c07 a008 7c08 a101 7d09 7c00 a009 7c09  |...|...}.|...|.
+000013f0: 6401 a102 0100 7144 7120 7110 7108 6400  d.....qDq q.q.d.
+00001400: 5300 2902 4e72 4500 0000 290a 721f 0000  S.).NrE...).r...
+00001410: 0072 0b00 0000 720e 0000 0072 1e00 0000  .r....r....r....
+00001420: 7220 0000 0072 0900 0000 7211 0000 0072  r ...r....r....r
+00001430: 1200 0000 5a1d 6765 745f 7372 6964 5f66  ....Z.get_srid_f
+00001440: 726f 6d5f 6765 6f6a 736f 6e5f 6665 6174  rom_geojson_feat
+00001450: 7572 6572 2100 0000 290a 722a 0000 0072  urer!...).r*...r
+00001460: 2f00 0000 722b 0000 0072 2c00 0000 722d  /...r+...r,...r-
+00001470: 0000 0072 2e00 0000 7222 0000 0072 3000  ...r....r"...r0.
+00001480: 0000 7239 0000 0072 3800 0000 7231 0000  ..r9...r8...r1..
+00001490: 0072 3100 0000 7232 0000 00da 2274 6573  .r1...r2...."tes
+000014a0: 745f 6765 745f 7372 6964 5f66 726f 6d5f  t_get_srid_from_
+000014b0: 6765 6f6a 736f 6e5f 6665 6174 7572 65dd  geojson_feature.
+000014c0: 0000 0073 1400 0000 0002 0402 0801 0802  ...s............
+000014d0: 0801 0802 1002 0802 0c02 0a02 7a33 5465  ............z3Te
+000014e0: 7374 4d61 7043 6c75 7374 6572 6572 2e74  stMapClusterer.t
+000014f0: 6573 745f 6765 745f 7372 6964 5f66 726f  est_get_srid_fro
+00001500: 6d5f 6765 6f6a 736f 6e5f 6665 6174 7572  m_geojson_featur
+00001510: 6563 0100 0000 0000 0000 0000 0000 0800  ec..............
+00001520: 0000 0700 0000 4300 0000 735a 0000 007c  ......C...sZ...|
+00001530: 00a0 00a1 007d 017c 0144 005d 487d 0274  .....}.|.D.]H}.t
+00001540: 017d 037c 00a0 0274 037c 0374 047c 02a1  .}.|...t.|.t.|..
+00001550: 047d 0474 057c 0483 017d 0567 007d 0274  .}.t.|...}.g.}.t
+00001560: 067d 067c 05a0 077c 067c 037c 02a1 037d  .}.|...|.|.|...}
+00001570: 077c 00a0 0874 097c 0783 0164 016b 04a1  .|...t.|...d.k..
+00001580: 0101 0071 0c64 0053 0072 4c00 0000 290a  ...q.d.S.rL...).
+00001590: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+000015a0: 0c00 0000 7210 0000 0072 0900 0000 7212  ....r....r....r.
+000015b0: 0000 005a 0c67 7269 645f 636c 7573 7465  ...Z.grid_cluste
+000015c0: 7272 2700 0000 7237 0000 0029 0872 2a00  rr'...r7...).r*.
+000015d0: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
+000015e0: 0072 2200 0000 7230 0000 0072 3900 0000  .r"...r0...r9...
+000015f0: da05 6365 6c6c 7372 3100 0000 7231 0000  ..cellsr1...r1..
+00001600: 0072 3200 0000 da11 7465 7374 5f67 7269  .r2.....test_gri
+00001610: 645f 636c 7573 7465 72f2 0000 0073 1200  d_cluster....s..
+00001620: 0000 0002 0801 0802 0401 1002 0802 0402  ................
+00001630: 0402 0e02 7a22 5465 7374 4d61 7043 6c75  ....z"TestMapClu
+00001640: 7374 6572 6572 2e74 6573 745f 6772 6964  sterer.test_grid
+00001650: 5f63 6c75 7374 6572 6301 0000 0000 0000  _clusterc.......
+00001660: 0000 0000 000a 0000 000a 0000 0043 0000  .............C..
+00001670: 0073 6c00 0000 7400 7d01 7401 4400 5d5e  .sl...t.}.t.D.]^
+00001680: 7d02 7402 4400 5d54 7d03 7c00 a003 a100  }.t.D.]T}.|.....
+00001690: 7d04 7c04 4400 5d42 7d05 7c00 a004 7c03  }.|.D.]B}.|...|.
+000016a0: 7c01 7c02 7c05 a104 7d06 7405 7c06 8301  |.|.|...}.t.|...
+000016b0: 7d07 7c07 a006 a100 7d08 6401 6402 6403  }.|.....}.d.d.d.
+000016c0: 6404 6405 6406 6407 6707 7d09 7c00 a007  d.d.d.d.g.}.|...
+000016d0: 7c08 7c09 a102 0100 7120 7110 7108 6400  |.|.....q q.q.d.
+000016e0: 5300 2908 4eda 0269 64da 046e 616d 65da  S.).N..id..name.
+000016f0: 0573 7479 6c65 da06 7261 7469 6e67 da0d  .style..rating..
+00001700: 6672 6565 5f65 6e74 7261 6e63 65da 0c6c  free_entrance..l
+00001710: 6173 745f 7265 6e65 7761 6cfa 1263 6f6f  ast_renewal..coo
+00001720: 7264 696e 6174 6573 3a3a 6279 7465 6129  rdinates::bytea)
+00001730: 0872 1f00 0000 720b 0000 0072 0e00 0000  .r....r....r....
+00001740: 721e 0000 0072 2000 0000 7209 0000 00da  r....r ...r.....
+00001750: 1367 6574 5f67 6973 5f66 6965 6c64 5f6e  .get_gis_field_n
+00001760: 616d 6573 7221 0000 0029 0a72 2a00 0000  amesr!...).r*...
+00001770: 722f 0000 0072 2b00 0000 722c 0000 0072  r/...r+...r,...r
+00001780: 2d00 0000 722e 0000 0072 2200 0000 7230  -...r....r"...r0
+00001790: 0000 00da 0b66 6965 6c64 5f6e 616d 6573  .....field_names
+000017a0: 5a14 6578 7065 6374 6564 5f66 6965 6c64  Z.expected_field
+000017b0: 5f6e 616d 6573 7231 0000 0072 3100 0000  _namesr1...r1...
+000017c0: 7232 0000 00da 1874 6573 745f 6765 745f  r2.....test_get_
+000017d0: 6769 735f 6669 656c 645f 6e61 6d65 7305  gis_field_names.
+000017e0: 0100 0073 1800 0000 0002 0402 0801 0802  ...s............
+000017f0: 0801 0802 1002 0802 0802 0c01 02ff 0403  ................
+00001800: 7a29 5465 7374 4d61 7043 6c75 7374 6572  z)TestMapCluster
+00001810: 6572 2e74 6573 745f 6765 745f 6769 735f  er.test_get_gis_
+00001820: 6669 656c 645f 6e61 6d65 7363 0100 0000  field_namesc....
+00001830: 0000 0000 0000 0000 0a00 0000 0900 0000  ................
+00001840: 4300 0000 735e 0000 0074 007d 0174 0144  C...s^...t.}.t.D
+00001850: 005d 507d 0274 0244 005d 467d 037c 00a0  .]P}.t.D.]F}.|..
+00001860: 03a1 007d 047c 0444 005d 347d 057c 00a0  ...}.|.D.]4}.|..
+00001870: 047c 037c 017c 027c 05a1 047d 0674 057c  .|.|.|.|...}.t.|
+00001880: 0683 017d 077c 07a0 06a1 007d 0864 017d  ...}.|.....}.d.}
+00001890: 097c 00a0 077c 087c 09a1 0201 0071 2071  .|...|.|.....q q
+000018a0: 1071 0864 0053 0029 024e 7a42 6964 2c6e  .q.d.S.).NzBid,n
+000018b0: 616d 652c 7374 796c 652c 7261 7469 6e67  ame,style,rating
+000018c0: 2c66 7265 655f 656e 7472 616e 6365 2c6c  ,free_entrance,l
+000018d0: 6173 745f 7265 6e65 7761 6c2c 636f 6f72  ast_renewal,coor
+000018e0: 6469 6e61 7465 733a 3a62 7974 6561 2908  dinates::bytea).
+000018f0: 721f 0000 0072 0b00 0000 720e 0000 0072  r....r....r....r
+00001900: 1e00 0000 7220 0000 0072 0900 0000 5a12  ....r ...r....Z.
+00001910: 6765 745f 6769 735f 6669 656c 6473 5f73  get_gis_fields_s
+00001920: 7472 7221 0000 0029 0a72 2a00 0000 722f  trr!...).r*...r/
+00001930: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00001940: 0000 722e 0000 0072 2200 0000 7230 0000  ..r....r"...r0..
+00001950: 005a 0a66 6965 6c64 735f 7374 725a 0c65  .Z.fields_strZ.e
+00001960: 7870 6563 7465 645f 7374 7272 3100 0000  xpected_strr1...
+00001970: 7231 0000 0072 3200 0000 da16 7465 7374  r1...r2.....test
+00001980: 5f67 6574 5f67 6973 5f66 6965 6c64 5f73  _get_gis_field_s
+00001990: 7472 1b01 0000 7314 0000 0000 0204 0208  tr....s.........
+000019a0: 0108 0308 0108 0210 0208 0208 0104 027a  ...............z
+000019b0: 2754 6573 744d 6170 436c 7573 7465 7265  'TestMapClustere
+000019c0: 722e 7465 7374 5f67 6574 5f67 6973 5f66  r.test_get_gis_f
+000019d0: 6965 6c64 5f73 7472 6301 0000 0000 0000  ield_strc.......
+000019e0: 0000 0000 000f 0000 000b 0000 0043 0000  .............C..
+000019f0: 0073 f200 0000 6401 7d01 7400 4400 5de4  .s....d.}.t.D.].
+00001a00: 7d02 7401 4400 5dda 7d03 7c00 a002 a100  }.t.D.].}.|.....
+00001a10: 7d04 7c04 4400 5dc8 7d05 7c00 a003 7c03  }.|.D.].}.|...|.
+00001a20: 7c01 7c02 7c05 a104 7d06 7404 7c06 8301  |.|.|...}.t.|...
+00001a30: 7d07 7405 7d08 6700 7d05 7c07 a006 7c08  }.t.}.g.}.|...|.
+00001a40: 7c03 7c01 7c05 a104 7d09 7c03 7407 6b02  |.|.|...}.|.t.k.
+00001a50: 7270 7c00 a008 7409 7c07 6a0a 6a0b 8301  rp|...t.|.j.j...
+00001a60: 6401 a102 0100 7c00 a00c 7409 7c09 8301  d.....|...t.|...
+00001a70: 6402 6b04 a101 0100 7c09 6402 1900 7d0a  d.k.....|.d...}.
+00001a80: 7c0a 6403 1900 7d0b 7c0a 6404 1900 6405  |.d...}.|.d...d.
+00001a90: 1900 7d0c 7c0a 6404 1900 6406 1900 7d0d  ..}.|.d...d...}.
+00001aa0: 7c07 a00d 7c03 7c0b 7c0c 7c0d 7c05 7c01  |...|.|.|.|.|.|.
+00001ab0: a106 7d0e 7c00 a00c 7c0a 6407 1900 6402  ..}.|...|.d...d.
+00001ac0: 6b04 a101 0100 7c00 a008 7409 740e 7c0e  k.....|...t.t.|.
+00001ad0: 8301 8301 7c0a 6407 1900 a102 0100 7120  ....|.d.......q 
+00001ae0: 7110 7108 6400 5300 2908 4e72 3400 0000  q.q.d.S.).Nr4...
+00001af0: 7201 0000 00da 0369 6473 da06 6365 6e74  r......ids..cent
+00001b00: 6572 da01 78da 0179 da05 636f 756e 7429  er..x..y..count)
+00001b10: 0f72 0b00 0000 720e 0000 0072 1e00 0000  .r....r....r....
+00001b20: 7220 0000 0072 0900 0000 7212 0000 0072  r ...r....r....r
+00001b30: 4d00 0000 720d 0000 0072 2100 0000 7237  M...r....r!...r7
+00001b40: 0000 0072 2200 0000 da0a 6765 6f6d 6574  ...r".....geomet
+00001b50: 7269 6573 7227 0000 005a 1a67 6574 5f6b  riesr'...Z.get_k
+00001b60: 6d65 616e 735f 636c 7573 7465 725f 636f  means_cluster_co
+00001b70: 6e74 656e 7472 2900 0000 290f 722a 0000  ntentr)...).r*..
+00001b80: 0072 2f00 0000 722b 0000 0072 2c00 0000  .r/...r+...r,...
+00001b90: 722d 0000 0072 2e00 0000 7222 0000 0072  r-...r....r"...r
+00001ba0: 3000 0000 7239 0000 0072 4e00 0000 da06  0...r9...rN.....
+00001bb0: 6d61 726b 6572 725e 0000 0072 6000 0000  markerr^...r`...
+00001bc0: 7261 0000 005a 0f63 6c75 7374 6572 5f63  ra...Z.cluster_c
+00001bd0: 6f6e 7465 6e74 7231 0000 0072 3100 0000  ontentr1...r1...
+00001be0: 7232 0000 00da 1f74 6573 745f 6765 745f  r2.....test_get_
+00001bf0: 6b6d 6561 6e73 5f63 6c75 7374 6572 5f63  kmeans_cluster_c
+00001c00: 6f6e 7465 6e74 3001 0000 7328 0000 0000  ontent0...s(....
+00001c10: 0204 0208 0108 0308 0108 0210 0208 0204  ................
+00001c20: 0204 0210 0208 0114 0212 0208 0208 010c  ................
+00001c30: 010c 0214 0212 017a 3054 6573 744d 6170  .......z0TestMap
+00001c40: 436c 7573 7465 7265 722e 7465 7374 5f67  Clusterer.test_g
+00001c50: 6574 5f6b 6d65 616e 735f 636c 7573 7465  et_kmeans_cluste
+00001c60: 725f 636f 6e74 656e 7463 0100 0000 0000  r_contentc......
+00001c70: 0000 0000 0000 0a00 0000 0900 0000 4300  ..............C.
+00001c80: 0000 736e 0000 0064 017d 0174 0044 005d  ..sn...d.}.t.D.]
+00001c90: 607d 0274 0144 005d 567d 037c 00a0 02a1  `}.t.D.]V}.|....
+00001ca0: 007d 047c 0444 005d 447d 057c 00a0 037c  .}.|.D.]D}.|...|
+00001cb0: 037c 017c 027c 05a1 047d 0674 047c 0683  .|.|.|...}.t.|..
+00001cc0: 017d 0774 057d 0867 007d 057c 07a0 067c  .}.t.}.g.}.|...|
+00001cd0: 087c 05a1 027d 097c 00a0 0774 0874 097c  .|...}.|...t.t.|
+00001ce0: 0983 0183 0164 02a1 0201 0071 2071 1071  .....d.....q q.q
+00001cf0: 0864 0053 0029 034e 7234 0000 00e9 6400  .d.S.).Nr4....d.
+00001d00: 0000 290a 720b 0000 0072 0e00 0000 721e  ..).r....r....r.
+00001d10: 0000 0072 2000 0000 7209 0000 0072 1200  ...r ...r....r..
+00001d20: 0000 5a10 6765 745f 6172 6561 5f63 6f6e  ..Z.get_area_con
+00001d30: 7465 6e74 7221 0000 0072 3700 0000 7229  tentr!...r7...r)
+00001d40: 0000 0029 0a72 2a00 0000 722f 0000 0072  ...).r*...r/...r
+00001d50: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+00001d60: 0000 0072 2200 0000 7230 0000 0072 3900  ...r"...r0...r9.
+00001d70: 0000 5a0c 6172 6561 5f63 6f6e 7465 6e74  ..Z.area_content
+00001d80: 7231 0000 0072 3100 0000 7232 0000 00da  r1...r1...r2....
+00001d90: 1574 6573 745f 6765 745f 6172 6561 5f63  .test_get_area_c
+00001da0: 6f6e 7465 6e74 5601 0000 7316 0000 0000  ontentV...s.....
+00001db0: 0204 0208 0108 0308 0108 0210 0208 0204  ................
+00001dc0: 0104 020c 027a 2654 6573 744d 6170 436c  .....z&TestMapCl
+00001dd0: 7573 7465 7265 722e 7465 7374 5f67 6574  usterer.test_get
+00001de0: 5f61 7265 615f 636f 6e74 656e 7463 0100  _area_contentc..
+00001df0: 0000 0000 0000 0000 0000 0b00 0000 0900  ................
+00001e00: 0000 4300 0000 7364 0000 0064 017d 0174  ..C...sd...d.}.t
+00001e10: 0044 005d 567d 0274 0144 005d 4c7d 037c  .D.]V}.t.D.]L}.|
+00001e20: 00a0 02a1 007d 047c 0444 005d 3a7d 057c  .....}.|.D.]:}.|
+00001e30: 00a0 037c 037c 017c 027c 05a1 047d 0674  ...|.|.|.|...}.t
+00001e40: 047c 0683 017d 0774 057d 087c 07a0 067c  .|...}.t.}.|...|
+00001e50: 08a1 017d 0964 027d 0a7c 00a0 077c 097c  ...}.d.}.|...|.|
+00001e60: 0aa1 0201 0071 2071 1071 0864 0053 0029  .....q q.q.d.S.)
+00001e70: 034e 7234 0000 0061 0301 0000 2820 5354  .Nr4...a....( ST
+00001e80: 5f49 6e74 6572 7365 6374 7328 636f 6f72  _Intersects(coor
+00001e90: 6469 6e61 7465 732c 2053 545f 4765 6f6d  dinates, ST_Geom
+00001ea0: 6574 7279 4672 6f6d 5465 7874 2827 504f  etryFromText('PO
+00001eb0: 4c59 474f 4e20 2828 3939 3038 3532 2e35  LYGON ((990852.5
+00001ec0: 3438 3139 3339 3934 3120 3635 3339 3635  481939941 653965
+00001ed0: 302e 3638 3930 3732 3839 392c 2039 3930  0.689072899, 990
+00001ee0: 3835 322e 3534 3831 3933 3939 3431 2035  852.5481939941 5
+00001ef0: 3938 3032 3237 2e31 3032 3032 3834 3238  980227.102028428
+00001f00: 2c20 3135 3539 3837 362e 3232 3739 3935  , 1559876.227995
+00001f10: 3930 3238 2035 3938 3032 3237 2e31 3032  9028 5980227.102
+00001f20: 3032 3834 3238 2c20 3135 3539 3837 362e  028428, 1559876.
+00001f30: 3232 3739 3935 3930 3238 2036 3533 3936  2279959028 65396
+00001f40: 3530 2e36 3839 3037 3238 3939 2c20 3939  50.689072899, 99
+00001f50: 3038 3532 2e35 3438 3139 3339 3934 3120  0852.5481939941 
+00001f60: 3635 3339 3635 302e 3638 3930 3732 3839  6539650.68907289
+00001f70: 3929 2927 2c20 3338 3537 2920 2920 2929  9))', 3857) ) ))
+00001f80: 0872 0b00 0000 720e 0000 0072 1e00 0000  .r....r....r....
+00001f90: 7220 0000 0072 0900 0000 7212 0000 005a  r ...r....r....Z
+00001fa0: 1567 6574 5f67 656f 6d5f 6669 6c74 6572  .get_geom_filter
+00001fb0: 7374 7269 6e67 7221 0000 0029 0b72 2a00  stringr!...).r*.
+00001fc0: 0000 722f 0000 0072 2b00 0000 722c 0000  ..r/...r+...r,..
+00001fd0: 0072 2d00 0000 722e 0000 0072 2200 0000  .r-...r....r"...
+00001fe0: 7230 0000 0072 3900 0000 5a11 6765 6f6d  r0...r9...Z.geom
+00001ff0: 5f66 696c 7465 7273 7472 696e 67da 0f65  _filterstring..e
+00002000: 7870 6563 7465 645f 7374 7269 6e67 7231  xpected_stringr1
+00002010: 0000 0072 3100 0000 7232 0000 00da 1a74  ...r1...r2.....t
+00002020: 6573 745f 6765 745f 6765 6f6d 5f66 696c  est_get_geom_fil
+00002030: 7465 7273 7472 696e 676d 0100 0073 1600  terstringm...s..
+00002040: 0000 0002 0402 0801 0803 0801 0802 1002  ................
+00002050: 0802 0402 0a02 0402 7a2b 5465 7374 4d61  ........z+TestMa
+00002060: 7043 6c75 7374 6572 6572 2e74 6573 745f  pClusterer.test_
+00002070: 6765 745f 6765 6f6d 5f66 696c 7465 7273  get_geom_filters
+00002080: 7472 696e 6763 0100 0000 0000 0000 0000  tringc..........
+00002090: 0000 0c00 0000 0900 0000 4300 0000 7388  ..........C...s.
+000020a0: 0000 0064 017d 0174 0044 005d 7a7d 0274  ...d.}.t.D.]z}.t
+000020b0: 0144 005d 707d 037c 00a0 02a1 007d 047c  .D.]p}.|.....}.|
+000020c0: 0444 005d 5e7d 057c 00a0 037c 037c 017c  .D.]^}.|...|.|.|
+000020d0: 027c 05a1 047d 0674 047c 0683 017d 0774  .|...}.t.|...}.t
+000020e0: 057d 087c 07a0 067c 0864 027c 01a1 037d  .}.|...|.d.|...}
+000020f0: 097c 00a0 0774 087c 0983 0164 03a1 0201  .|...t.|...d....
+00002100: 007c 0964 0419 007d 0a7c 07a0 097c 0a7c  .|.d...}.|...|.|
+00002110: 01a1 027d 0b7c 00a0 077c 0b64 05a1 0201  ...}.|...|.d....
+00002120: 0071 2071 1071 0864 0053 0029 064e e90a  .q q.q.d.S.).N..
+00002130: 0000 00da 0461 7265 6172 3400 0000 7201  .....arear4...r.
+00002140: 0000 00e9 1e00 0000 290a 720b 0000 0072  ........).r....r
+00002150: 0e00 0000 721e 0000 0072 2000 0000 7209  ....r....r ...r.
+00002160: 0000 0072 1100 0000 7241 0000 0072 2100  ...r....rA...r!.
+00002170: 0000 7237 0000 005a 0b63 616c 6375 6c61  ..r7...Z.calcula
+00002180: 7465 5f6b 290c 722a 0000 0072 2f00 0000  te_k).r*...r/...
+00002190: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
+000021a0: 2e00 0000 7222 0000 0072 3000 0000 7239  ....r"...r0...r9
+000021b0: 0000 0072 3a00 0000 da04 6765 6f73 da01  ...r:.....geos..
+000021c0: 6b72 3100 0000 7231 0000 0072 3200 0000  kr1...r1...r2...
+000021d0: da10 7465 7374 5f63 616c 6375 6c61 7465  ..test_calculate
+000021e0: 5f6b 8501 0000 731a 0000 0000 0204 0208  _k....s.........
+000021f0: 0108 0208 0108 0210 0208 0204 020e 0210  ................
+00002200: 0208 020c 027a 2154 6573 744d 6170 436c  .....z!TestMapCl
+00002210: 7573 7465 7265 722e 7465 7374 5f63 616c  usterer.test_cal
+00002220: 6375 6c61 7465 5f6b 6301 0000 0000 0000  culate_kc.......
+00002230: 0000 0000 000b 0000 0009 0000 0043 0000  .............C..
+00002240: 0073 c800 0000 7400 7d01 7401 4400 5dba  .s....t.}.t.D.].
+00002250: 7d02 7402 4400 5db0 7d03 7c00 a003 a100  }.t.D.].}.|.....
+00002260: 7d04 7c04 4400 5d9e 7d05 7c00 a004 7c02  }.|.D.].}.|...|.
+00002270: 7c01 7c03 7c05 a104 7d06 7405 7c06 8301  |.|.|...}.t.|...
+00002280: 7d07 7406 7d08 7c07 a007 7c08 7c02 7c01  }.t.}.|...|.|.|.
+00002290: a103 7d09 7c00 a008 7409 7c09 8301 6401  ..}.|...t.|...d.
+000022a0: 6b04 a101 0100 7c00 a00a 7c07 6a0b 6a0c  k.....|...|.j.j.
+000022b0: 7c01 a102 0100 7c00 a00a 7c07 6a0b 6a0d  |.....|...|.j.j.
+000022c0: 7c03 a102 0100 7c00 a00a 7c07 6a0b 6a0e  |.....|...|.j.j.
+000022d0: 7c02 a102 0100 7c00 a00a 7c07 6a0b 6a0f  |.....|...|.j.j.
+000022e0: 7c05 a102 0100 7c07 a007 7c08 7c02 7c01  |.....|...|.|.|.
+000022f0: a103 7d0a 7c00 a00a 7409 7c0a 8301 6401  ..}.|...t.|...d.
+00002300: a102 0100 7120 7110 7108 6400 5300 724c  ....q q.q.d.S.rL
+00002310: 0000 0029 1072 1f00 0000 720e 0000 0072  ...).r....r....r
+00002320: 0b00 0000 721e 0000 0072 2000 0000 7209  ....r....r ...r.
+00002330: 0000 0072 1200 0000 7241 0000 0072 2700  ...r....rA...r'.
+00002340: 0000 7237 0000 0072 2100 0000 7222 0000  ..r7...r!...r"..
+00002350: 0072 2f00 0000 722b 0000 0072 2c00 0000  .r/...r+...r,...
+00002360: 722e 0000 0029 0b72 2a00 0000 722f 0000  r....).r*...r/..
+00002370: 0072 2c00 0000 722b 0000 0072 2d00 0000  .r,...r+...r-...
+00002380: 722e 0000 0072 2200 0000 7230 0000 0072  r....r"...r0...r
+00002390: 3900 0000 7242 0000 005a 1863 6163 6865  9...rB...Z.cache
+000023a0: 5f63 6c75 7374 6572 5f67 656f 6d65 7472  _cluster_geometr
+000023b0: 6965 7372 3100 0000 7231 0000 0072 3200  iesr1...r1...r2.
+000023c0: 0000 da17 7465 7374 5f73 616d 655f 7265  ....test_same_re
+000023d0: 7175 6573 745f 7477 6963 65a0 0100 0073  quest_twice....s
+000023e0: 3000 0000 0002 0402 0801 0803 0801 0802  0...............
+000023f0: 1002 0802 0402 0401 0200 0200 02ff 0403  ................
+00002400: 1201 1001 1001 1001 1002 0401 0200 0200  ................
+00002410: 02ff 0403 7a28 5465 7374 4d61 7043 6c75  ....z(TestMapClu
+00002420: 7374 6572 6572 2e74 6573 745f 7361 6d65  sterer.test_same
+00002430: 5f72 6571 7565 7374 5f74 7769 6365 6301  _request_twicec.
+00002440: 0000 0000 0000 0000 0000 0008 0000 0008  ................
+00002450: 0000 0043 0000 0073 7a00 0000 7400 6a01  ...C...sz...t.j.
+00002460: a002 a100 a003 a100 7d01 7c00 a004 a100  ........}.|.....
+00002470: 7d02 7c02 4400 5d5a 7d03 7c00 a005 7406  }.|.D.]Z}.|...t.
+00002480: 7407 7408 7c03 a104 7d04 7409 7c04 8301  t.t.|...}.t.|...
+00002490: 7d05 7c05 a00a 7c01 6a0b a101 7d06 7c05  }.|...|.j...}.|.
+000024a0: a00c a100 4400 5d28 7d07 7c07 6401 6b02  ....D.](}.|.d.k.
+000024b0: 725a 6402 7d07 7c00 a00d 740e 7c01 7c07  rZd.}.|...t.|.|.
+000024c0: 8302 740e 7c06 7c07 8302 a102 0100 714a  ..t.|.|.......qJ
+000024d0: 711a 6400 5300 2903 4e72 5900 0000 da0b  q.d.S.).NrY.....
+000024e0: 636f 6f72 6469 6e61 7465 7329 0f72 1800  coordinates).r..
+000024f0: 0000 da07 6f62 6a65 6374 73da 0361 6c6c  ....objects..all
+00002500: da05 6669 7273 7472 1e00 0000 7220 0000  ..firstr....r ..
+00002510: 0072 0c00 0000 721f 0000 0072 1000 0000  .r....r....r....
+00002520: 7209 0000 005a 1367 6574 5f64 6174 6173  r....Z.get_datas
+00002530: 6574 5f63 6f6e 7465 6e74 7253 0000 0072  et_contentrS...r
+00002540: 5a00 0000 7221 0000 00da 0767 6574 6174  Z...r!.....getat
+00002550: 7472 2908 722a 0000 00da 0667 6172 6465  tr).r*.....garde
+00002560: 6e72 2d00 0000 722e 0000 0072 2200 0000  nr-...r....r"...
+00002570: 7230 0000 005a 0767 6172 6465 6e5f da0a  r0...Z.garden_..
+00002580: 6669 656c 645f 6e61 6d65 7231 0000 0072  field_namer1...r
+00002590: 3100 0000 7232 0000 00da 1874 6573 745f  1...r2.....test_
+000025a0: 6765 745f 6461 7461 7365 745f 636f 6e74  get_dataset_cont
+000025b0: 656e 74c0 0100 0073 1400 0000 0002 0e02  ent....s........
+000025c0: 0801 0802 1001 0802 0c02 0c02 0801 0402  ................
+000025d0: 7a29 5465 7374 4d61 7043 6c75 7374 6572  z)TestMapCluster
+000025e0: 6572 2e74 6573 745f 6765 745f 6461 7461  er.test_get_data
+000025f0: 7365 745f 636f 6e74 656e 7463 0100 0000  set_contentc....
+00002600: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00002610: 4300 0000 7304 0000 0064 0053 0072 3d00  C...s....d.S.r=.
+00002620: 0000 7231 0000 00a9 0172 2a00 0000 7231  ..r1.....r*...r1
+00002630: 0000 0072 3100 0000 7232 0000 00da 1374  ...r1...r2.....t
+00002640: 6573 745f 7061 6e6e 6564 5f72 6571 7565  est_panned_reque
+00002650: 7374 d301 0000 7302 0000 0000 017a 2454  st....s......z$T
+00002660: 6573 744d 6170 436c 7573 7465 7265 722e  estMapClusterer.
+00002670: 7465 7374 5f70 616e 6e65 645f 7265 7175  test_panned_requ
+00002680: 6573 7463 0100 0000 0000 0000 0000 0000  estc............
+00002690: 0100 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000026a0: 0064 0053 0072 3d00 0000 7231 0000 0072  .d.S.r=...r1...r
+000026b0: 7900 0000 7231 0000 0072 3100 0000 7232  y...r1...r1...r2
+000026c0: 0000 00da 1774 6573 745f 7a6f 6f6d 5f6c  .....test_zoom_l
+000026d0: 6576 656c 5f63 6861 6e67 6564 d601 0000  evel_changed....
+000026e0: 7302 0000 0000 017a 2854 6573 744d 6170  s......z(TestMap
+000026f0: 436c 7573 7465 7265 722e 7465 7374 5f7a  Clusterer.test_z
+00002700: 6f6f 6d5f 6c65 7665 6c5f 6368 616e 6765  oom_level_change
+00002710: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
+00002720: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
+00002730: 0053 0072 3d00 0000 7231 0000 0072 7900  .S.r=...r1...ry.
+00002740: 0000 7231 0000 0072 3100 0000 7232 0000  ..r1...r1...r2..
+00002750: 00da 1874 6573 745f 636c 7573 7465 7274  ...test_clustert
+00002760: 7970 655f 6368 616e 6765 64d9 0100 0073  ype_changed....s
+00002770: 0200 0000 0001 7a29 5465 7374 4d61 7043  ......z)TestMapC
+00002780: 6c75 7374 6572 6572 2e74 6573 745f 636c  lusterer.test_cl
+00002790: 7573 7465 7274 7970 655f 6368 616e 6765  ustertype_change
+000027a0: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
+000027b0: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
+000027c0: 0053 0072 3d00 0000 7231 0000 0072 7900  .S.r=...r1...ry.
+000027d0: 0000 7231 0000 0072 3100 0000 7232 0000  ..r1...r1...r2..
+000027e0: 00da 1074 6573 745f 636c 6561 725f 6361  ...test_clear_ca
+000027f0: 6368 65dc 0100 0073 0200 0000 0001 7a21  che....s......z!
+00002800: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
+00002810: 2e74 6573 745f 636c 6561 725f 6361 6368  .test_clear_cach
+00002820: 654e 2919 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
+00002830: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00002840: 616c 6e61 6d65 5f5f 7233 0000 0072 3500  alname__r3...r5.
+00002850: 0000 723c 0000 0072 3f00 0000 7240 0000  ..r<...r?...r@..
+00002860: 0072 4300 0000 724b 0000 0072 4f00 0000  .rC...rK...rO...
+00002870: 7250 0000 0072 5200 0000 725c 0000 0072  rP...rR...r\...r
+00002880: 5d00 0000 7265 0000 0072 6700 0000 7269  ]...re...rg...ri
+00002890: 0000 0072 6f00 0000 7270 0000 0072 7800  ...ro...rp...rx.
+000028a0: 0000 727a 0000 0072 7b00 0000 727c 0000  ..rz...r{...r|..
+000028b0: 0072 7d00 0000 7231 0000 0072 3100 0000  .r}...r1...r1...
+000028c0: 7231 0000 0072 3200 0000 721b 0000 0014  r1...r2...r.....
+000028d0: 0000 0073 2c00 0000 0803 0816 0812 0822  ...s,.........."
+000028e0: 0816 0813 0817 0825 0817 0815 0813 0816  .......%........
+000028f0: 0815 0826 0817 0818 081b 0820 0813 0803  ...&....... ....
+00002900: 0803 0803 721b 0000 0063 0000 0000 0000  ....r....c......
+00002910: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00002920: 0000 7334 0000 0065 005a 0164 005a 0264  ..s4...e.Z.d.Z.d
+00002930: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
+00002940: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
+00002950: 0964 0a84 005a 0764 0b53 0029 0cda 1d54  .d...Z.d.S.)...T
+00002960: 6573 744d 6170 436c 7573 7465 7265 7243  estMapClustererC
+00002970: 6f6e 7465 6e74 436f 756e 7473 6301 0000  ontentCountsc...
+00002980: 0000 0000 0000 0000 000d 0000 000a 0000  ................
+00002990: 0043 0000 0073 6e01 0000 6401 7d01 6402  .C...sn...d.}.d.
+000029a0: 6403 6404 6405 9c03 6701 7d02 6406 6407  d.d.d...g.}.d.d.
+000029b0: 6408 6404 6405 9c03 6701 6901 6406 6407  d.d.d...g.i.d.d.
+000029c0: 6408 6409 6405 9c03 6701 6901 640a 9c02  d.d.d...g.i.d...
+000029d0: 7d03 7400 4400 9001 5d2a 7d04 7401 4400  }.t.D...]*}.t.D.
+000029e0: 9001 5d1e 7d05 7402 7403 7404 7405 6604  ..].}.t.t.t.t.f.
+000029f0: 4400 9001 5d0a 7d06 7c04 7406 6b02 7270  D...].}.|.t.k.rp
+00002a00: 7c05 7407 6b03 7270 7158 7c05 7407 6b02  |.t.k.rpqX|.t.k.
+00002a10: 7282 7c06 7403 6b03 7282 7158 7c00 a008  r.|.t.k.r.qX|...
+00002a20: 7c05 7c01 7c04 7c02 a104 7d07 7409 7c07  |.|.|.|...}.t.|.
+00002a30: 740a 640b 8d02 7d08 7c08 a00b 7c06 7c05  t.d...}.|...|.|.
+00002a40: 7c02 7c01 7c03 a105 7d09 640c 640d 640c  |.|.|...}.d.d.d.
+00002a50: 6901 640d 640c 6901 640a 9c02 640e 9c02  i.d.d.i.d...d...
+00002a60: 7d0a 7c00 a00c 7c09 7c0a a102 0100 7c05  }.|...|.|.....|.
+00002a70: 7407 6b02 9001 722c 7c00 a00d 640f 6403  t.k...r,|...d.d.
+00002a80: a102 0100 7c00 a00d 6410 6411 a102 0100  ....|...d.d.....
+00002a90: 7c08 a00b 7c06 7c05 7c02 7c01 7c03 a105  |...|.|.|.|.|...
+00002aa0: 7d09 6412 640d 640c 6901 640d 6412 6901  }.d.d.d.i.d.d.i.
+00002ab0: 640a 9c02 640e 9c02 7d0a 7c00 a00c 7c09  d...d...}.|...|.
+00002ac0: 7c0a a102 0100 740e 6a0f a010 a100 7d0b  |.....t.j.....}.
+00002ad0: 7c0b 4400 5d0e 7d0c 7c0c a011 a100 0100  |.D.].}.|.......
+00002ae0: 9001 713a 740e 6a0f a010 a100 7d0b 7c00  ..q:t.j.....}.|.
+00002af0: a00c 7c0b a012 a100 640c a102 0100 7158  ..|.....d.....qX
+00002b00: 7146 713c 6400 5300 2913 4e72 6a00 0000  qFq<d.S.).Nrj...
+00002b10: 7255 0000 00da 0573 746f 6e65 fa01 3da9  rU.....stone..=.
+00002b20: 03da 0663 6f6c 756d 6eda 0576 616c 7565  ...column..value
+00002b30: da08 6f70 6572 6174 6f72 722e 0000 0072  ..operatorr....r
+00002b40: 5700 0000 547a 0221 3d29 02da 0466 7265  W...Tz.!=)...fre
+00002b50: 655a 0470 6169 64a9 0172 2500 0000 7201  eZ.paid..r%...r.
+00002b60: 0000 0072 6200 0000 2902 7262 0000 00da  ...rb...).rb....
+00002b70: 0b6d 6f64 756c 6174 696f 6e73 fa06 6e61  .modulations..na
+00002b80: 6d65 2031 fa06 6e61 6d65 2032 da06 666c  me 1..name 2..fl
+00002b90: 6f77 6572 7234 0000 0029 1372 0b00 0000  owerr4...).r....
+00002ba0: 720e 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00002bb0: 1300 0000 7214 0000 0072 1000 0000 720c  ....r....r....r.
+00002bc0: 0000 0072 2000 0000 7209 0000 00da 0e54  ...r ...r......T
+00002bd0: 4553 545f 4752 4944 5f53 495a 455a 1667  EST_GRID_SIZEZ.g
+00002be0: 6574 5f6d 6170 5f63 6f6e 7465 6e74 5f63  et_map_content_c
+00002bf0: 6f75 6e74 7372 2100 0000 da0c 6372 6561  ountsr!.....crea
+00002c00: 7465 5f70 6f69 6e74 7218 0000 0072 7200  te_pointr....rr.
+00002c10: 0000 7273 0000 00da 0664 656c 6574 6572  ..rs.....deleter
+00002c20: 6200 0000 290d 722a 0000 0072 2f00 0000  b...).r*...r/...
+00002c30: 722e 0000 0072 8a00 0000 722b 0000 0072  r....r....r+...r
+00002c40: 2c00 0000 7239 0000 0072 2200 0000 7230  ,...r9...r"...r0
+00002c50: 0000 00da 0672 6573 756c 74da 0f65 7870  .....result..exp
+00002c60: 6563 7465 645f 7265 7375 6c74 da07 6761  ected_result..ga
+00002c70: 7264 656e 7372 7600 0000 7231 0000 0072  rdensrv...r1...r
+00002c80: 3100 0000 7232 0000 00da 1a74 6573 745f  1...r2.....test_
+00002c90: 6765 745f 6d61 705f 636f 6e74 656e 745f  get_map_content_
+00002ca0: 636f 756e 74e2 0100 0073 7800 0000 0002  count....sx.....
+00002cb0: 0405 0201 0201 02fd 04ff 040b 0202 0201  ................
+00002cc0: 0201 02fd 04ff 02fe 020b 0202 0201 0201  ................
+00002cd0: 02fd 04ff 02ff 02f5 0617 0a01 0a02 1202  ................
+00002ce0: 1001 0202 1001 0202 1001 0c02 1203 0203  ................
+00002cf0: 0200 02ff 0204 0200 02ff 02fc 04fe 060b  ................
+00002d00: 0c02 0a02 0c01 0c02 1203 0203 0200 02ff  ................
+00002d10: 0204 0200 02ff 02fc 04fe 060e 0c02 0a01  ................
+00002d20: 0801 0c03 0a02 7a38 5465 7374 4d61 7043  ......z8TestMapC
+00002d30: 6c75 7374 6572 6572 436f 6e74 656e 7443  lustererContentC
+00002d40: 6f75 6e74 732e 7465 7374 5f67 6574 5f6d  ounts.test_get_m
+00002d50: 6170 5f63 6f6e 7465 6e74 5f63 6f75 6e74  ap_content_count
+00002d60: 6301 0000 0000 0000 0000 0000 000c 0000  c...............
+00002d70: 0006 0000 0043 0000 0073 3201 0000 6401  .....C...s2...d.
+00002d80: 7d01 7400 7d02 7401 7d03 6700 7d04 7c00  }.t.}.t.}.g.}.|.
+00002d90: a002 7c02 7c01 7c03 7c04 a104 7d05 7403  ..|.|.|.|...}.t.
+00002da0: 7c05 7404 6402 8d02 7d06 7405 7d07 7c06  |.t.d...}.t.}.|.
+00002db0: a006 7c07 7c02 7c01 a103 7d08 7c06 a007  ..|.|.|...}.|...
+00002dc0: 7c08 7c04 a102 7d09 7c00 a008 7c09 6403  |.|...}.|...|.d.
+00002dd0: a102 0100 7c00 a009 6404 6405 a102 0100  ....|...d.d.....
+00002de0: 7c06 a007 7c08 7c04 a102 7d09 7c00 a008  |...|.|...}.|...
+00002df0: 7c09 6406 a102 0100 7c00 a009 6407 6408  |.d.....|...d.d.
+00002e00: a102 0100 7c06 a007 7c08 7c04 a102 7d09  ....|...|.|...}.
+00002e10: 7c00 a008 7c09 6409 a102 0100 640a 6405  |...|.d.....d.d.
+00002e20: 640b 640c 9c03 6701 7d04 7c06 a007 7c08  d.d...g.}.|...|.
+00002e30: 7c04 a102 7d09 7c00 a008 7c09 6406 a102  |...}.|...|.d...
+00002e40: 0100 640a 6405 640b 640c 9c03 640a 6408  ..d.d.d.d...d.d.
+00002e50: 640b 640d 640e 9c04 6702 7d04 7c06 a007  d.d.d...g.}.|...
+00002e60: 7c08 7c04 a102 7d09 7c00 a008 7c09 6409  |.|...}.|...|.d.
+00002e70: a102 0100 740a 6a0b a00c a100 7d0a 7c0a  ....t.j.....}.|.
+00002e80: 4400 5d0e 7d0b 7c0b a00d a100 0100 9001  D.].}.|.........
+00002e90: 7104 740a 6a0b a00c a100 7d0a 7c00 a008  q.t.j.....}.|...
+00002ea0: 7c0a a00e a100 6403 a102 0100 6400 5300  |.....d.....d.S.
+00002eb0: 290f 4e72 6a00 0000 7289 0000 0072 0100  ).Nrj...r....r..
+00002ec0: 0000 728b 0000 0072 8200 0000 7234 0000  ..r....r....r4..
+00002ed0: 0072 8c00 0000 728d 0000 0072 3600 0000  .r....r....r6...
+00002ee0: 7255 0000 0072 8300 0000 7284 0000 00da  rU...r....r.....
+00002ef0: 024f 5229 0472 8500 0000 7286 0000 0072  .OR).r....r....r
+00002f00: 8700 0000 da0f 6c6f 6769 6361 6c4f 7065  ......logicalOpe
+00002f10: 7261 746f 7229 0f72 0c00 0000 720f 0000  rator).r....r...
+00002f20: 0072 2000 0000 7209 0000 0072 8e00 0000  .r ...r....r....
+00002f30: 7212 0000 00da 1b67 6574 5f67 656f 6d65  r......get_geome
+00002f40: 7472 6965 735f 666f 725f 636f 756e 7469  tries_for_counti
+00002f50: 6e67 5a17 7175 6572 795f 6d61 705f 636f  ngZ.query_map_co
+00002f60: 6e74 656e 745f 636f 756e 7472 2100 0000  ntent_countr!...
+00002f70: 728f 0000 0072 1800 0000 7272 0000 0072  r....r....rr...r
+00002f80: 7300 0000 7290 0000 0072 6200 0000 290c  s...r....rb...).
+00002f90: 722a 0000 0072 2f00 0000 722c 0000 0072  r*...r/...r,...r
+00002fa0: 2b00 0000 722e 0000 0072 2200 0000 7230  +...r....r"...r0
+00002fb0: 0000 0072 3900 0000 5a17 6765 6f6d 6574  ...r9...Z.geomet
+00002fc0: 7269 6573 5f66 6f72 5f63 6f75 6e74 696e  ries_for_countin
+00002fd0: 6772 6200 0000 7293 0000 0072 7600 0000  grb...r....rv...
+00002fe0: 7231 0000 0072 3100 0000 7232 0000 00da  r1...r1...r2....
+00002ff0: 1c74 6573 745f 7175 6572 795f 6d61 705f  .test_query_map_
+00003000: 636f 6e74 656e 745f 636f 756e 7444 0200  content_countD..
+00003010: 0073 5000 0000 0002 0401 0401 0403 0402  .sP.............
+00003020: 1001 0c02 0402 0e02 0c01 0c02 0c02 0c01  ................
+00003030: 0c02 0c02 0c01 0c05 0201 0201 02fd 04ff  ................
+00003040: 0408 0c01 0c04 0201 0201 02fd 0406 0201  ................
+00003050: 0201 0201 02fc 04fa 040e 0c01 0c02 0a01  ................
+00003060: 0801 0c03 0a02 7a3a 5465 7374 4d61 7043  ......z:TestMapC
+00003070: 6c75 7374 6572 6572 436f 6e74 656e 7443  lustererContentC
+00003080: 6f75 6e74 732e 7465 7374 5f71 7565 7279  ounts.test_query
+00003090: 5f6d 6170 5f63 6f6e 7465 6e74 5f63 6f75  _map_content_cou
+000030a0: 6e74 6301 0000 0000 0000 0000 0000 000a  ntc.............
+000030b0: 0000 0009 0000 0043 0000 0073 aa00 0000  .......C...s....
+000030c0: 6401 7d01 7400 4400 5d9c 7d02 7401 4400  d.}.t.D.].}.t.D.
+000030d0: 5d92 7d03 7402 7403 7404 7405 6604 4400  ].}.t.t.t.t.f.D.
+000030e0: 5d80 7d04 7c02 7406 6b02 7236 7c03 7407  ].}.|.t.k.r6|.t.
+000030f0: 6b03 7236 7120 7c03 7407 6b02 7248 7c04  k.r6q |.t.k.rH|.
+00003100: 7403 6b03 7248 7120 6700 7d05 7c00 a008  t.k.rHq g.}.|...
+00003110: 7c03 7c01 7c02 7c05 a104 7d06 7409 7c06  |.|.|.|...}.t.|.
+00003120: 740a 6402 8d02 7d07 7c07 a00b 7c04 7c03  t.d...}.|...|.|.
+00003130: 7c01 a103 7d08 7c00 a00c 740d 7c08 740e  |...}.|...t.|.t.
+00003140: 8302 a101 0100 7c08 4400 5d14 7d09 7c00  ......|.D.].}.|.
+00003150: a00c 6403 7c09 6a0f 6b06 a101 0100 718a  ..d.|.j.k.....q.
+00003160: 7120 7110 7108 6400 5300 2904 4e72 6a00  q q.q.d.S.).Nrj.
+00003170: 0000 7289 0000 00da 0750 4f4c 5947 4f4e  ..r......POLYGON
+00003180: 2910 720b 0000 0072 0e00 0000 7211 0000  ).r....r....r...
+00003190: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+000031a0: 7210 0000 0072 0c00 0000 7220 0000 0072  r....r....r ...r
+000031b0: 0900 0000 728e 0000 0072 9700 0000 7227  ....r....r....r'
+000031c0: 0000 0072 2800 0000 7229 0000 00da 0377  ...r(...r).....w
+000031d0: 6b74 290a 722a 0000 0072 2f00 0000 722b  kt).r*...r/...r+
+000031e0: 0000 0072 2c00 0000 7239 0000 0072 2e00  ...r,...r9...r..
+000031f0: 0000 7222 0000 0072 3000 0000 723a 0000  ..r"...r0...r:..
+00003200: 0072 4400 0000 7231 0000 0072 3100 0000  .rD...r1...r1...
+00003210: 7232 0000 00da 2074 6573 745f 6765 745f  r2.... test_get_
+00003220: 6765 6f6d 6574 7269 6573 5f66 6f72 5f63  geometries_for_c
+00003230: 6f75 6e74 696e 6788 0200 0073 1e00 0000  ounting....s....
+00003240: 0002 0402 0801 0802 1002 1001 0202 1001  ................
+00003250: 0202 0402 1001 0c02 0e02 1002 0802 7a3e  ..............z>
+00003260: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
+00003270: 436f 6e74 656e 7443 6f75 6e74 732e 7465  ContentCounts.te
+00003280: 7374 5f67 6574 5f67 656f 6d65 7472 6965  st_get_geometrie
+00003290: 735f 666f 725f 636f 756e 7469 6e67 6301  s_for_countingc.
+000032a0: 0000 0000 0000 0000 0000 000a 0000 0008  ................
+000032b0: 0000 0043 0000 0073 8e00 0000 6700 7d01  ...C...s....g.}.
+000032c0: 6401 7d02 7400 4400 5d7c 7d03 7401 4400  d.}.t.D.]|}.t.D.
+000032d0: 5d72 7d04 7c00 a002 7c04 7c02 7c03 7c01  ]r}.|...|.|.|.|.
+000032e0: a104 7d05 7403 7c05 7404 6402 8d02 7d06  ..}.t.|.t.d...}.
+000032f0: 7c06 a005 7406 a101 7d07 7c06 a007 7c07  |...t...}.|...|.
+00003300: 7c02 a102 7d08 7c00 a008 7409 7c08 8301  |...}.|...t.|...
+00003310: 6403 a102 0100 7c00 a008 7c08 6a0a 6404  d.....|...|.j.d.
+00003320: a102 0100 7c08 a00b 6405 a101 0100 6406  ....|...d.....d.
+00003330: 7d09 7c00 a008 7c09 7409 7c08 8301 a102  }.|...|.t.|.....
+00003340: 0100 7114 710c 6400 5300 2907 4e72 6a00  ..q.q.d.S.).Nrj.
+00003350: 0000 7289 0000 007a a753 5249 443d 3338  ..r....z.SRID=38
+00003360: 3537 3b50 4f4c 5947 4f4e 2028 2839 3738  57;POLYGON ((978
+00003370: 3339 332e 3936 3230 3520 3539 3438 3633  393.96205 594863
+00003380: 352e 3238 3930 3136 2c20 3135 3635 3433  5.289016, 156543
+00003390: 302e 3333 3932 3820 3539 3438 3633 352e  0.33928 5948635.
+000033a0: 3238 3930 3136 2c20 3135 3635 3433 302e  289016, 1565430.
+000033b0: 3333 3932 3820 3635 3734 3830 372e 3432  33928 6574807.42
+000033c0: 3437 3238 2c20 3937 3833 3933 2e39 3632  4728, 978393.962
+000033d0: 3035 2036 3537 3438 3037 2e34 3234 3732  05 6574807.42472
+000033e0: 382c 2039 3738 3339 332e 3936 3230 3520  8, 978393.96205 
+000033f0: 3539 3438 3633 352e 3238 3930 3136 2929  5948635.289016))
+00003400: 721d 0000 0072 4500 0000 7ac5 5352 4944  r....rE...z.SRID
+00003410: 3d34 3332 363b 504f 4c59 474f 4e20 2828  =4326;POLYGON ((
+00003420: 382e 3738 3930 3632 3439 3939 3937 3720  8.7890624999977 
+00003430: 3437 2e30 3430 3138 3231 3433 3237 3838  47.0401821432788
+00003440: 392c 2031 342e 3036 3234 3939 3939 3939  9, 14.0624999999
+00003450: 3936 3332 2034 372e 3034 3031 3832 3134  9632 47.04018214
+00003460: 3332 3738 3839 2c20 3134 2e30 3632 3439  327889, 14.06249
+00003470: 3939 3939 3939 3633 3220 3530 2e37 3336  999999632 50.736
+00003480: 3435 3531 3335 3539 3039 2c20 382e 3738  4551355909, 8.78
+00003490: 3930 3632 3439 3939 3937 3720 3530 2e37  90624999977 50.7
+000034a0: 3336 3435 3531 3335 3539 3039 2c20 382e  364551355909, 8.
+000034b0: 3738 3930 3632 3439 3939 3937 3720 3437  7890624999977 47
+000034c0: 2e30 3430 3138 3231 3433 3237 3838 3929  .04018214327889)
+000034d0: 2929 0c72 0b00 0000 720e 0000 0072 2000  )).r....r....r .
+000034e0: 0000 7209 0000 0072 8e00 0000 723e 0000  ..r....r....r>..
+000034f0: 0072 1200 0000 5a15 736e 6170 5f76 6965  .r....Z.snap_vie
+00003500: 7770 6f72 745f 746f 5f67 7269 6472 2100  wport_to_gridr!.
+00003510: 0000 da03 7374 7272 3800 0000 7249 0000  ....strr8...rI..
+00003520: 0029 0a72 2a00 0000 722e 0000 0072 2f00  .).r*...r....r/.
+00003530: 0000 722b 0000 0072 2c00 0000 7222 0000  ..r+...r,...r"..
+00003540: 0072 3000 0000 723a 0000 005a 0e67 7269  .r0...r:...Z.gri
+00003550: 645f 7265 6374 616e 676c 655a 0c70 6f6c  d_rectangleZ.pol
+00003560: 7967 6f6e 5f34 3332 3672 3100 0000 7231  ygon_4326r1...r1
+00003570: 0000 0072 3200 0000 da1a 7465 7374 5f73  ...r2.....test_s
 00003580: 6e61 705f 7669 6577 706f 7274 5f74 6f5f  nap_viewport_to_
-00003590: 6772 6964 6301 0000 0000 0000 0000 0000  gridc...........
-000035a0: 000c 0000 000a 0000 0043 0000 0073 bc00  .........C...s..
-000035b0: 0000 6401 7d01 6700 7d02 7c00 a000 6402  ..d.}.g.}.|...d.
-000035c0: 6403 a102 0100 7c00 a000 6404 6405 a102  d.....|...d.d...
-000035d0: 0100 7401 4400 5d92 7d03 7402 4400 5d88  ..t.D.].}.t.D.].
-000035e0: 7d04 7403 7404 7405 7406 6604 4400 5d76  }.t.t.t.t.f.D.]v
-000035f0: 7d05 7c00 a007 7c04 7c01 7c03 7c02 a104  }.|...|.|.|.|...
-00003600: 7d06 7408 7c06 7409 6406 8d02 7d07 6407  }.t.|.t.d...}.d.
-00003610: 7d08 7c07 a00a 7c05 7c04 7c01 7c02 7c08  }.|...|.|.|.|.|.
-00003620: a105 7d09 7c04 740b 6b02 7298 6408 6409  ..}.|.t.k.r.d.d.
-00003630: 6901 6408 6409 6901 640a 9c02 7d0a 7c00  i.d.d.i.d...}.|.
-00003640: a00c 7c09 7c0a a102 0100 740d 6a0e a00f  ..|.|.....t.j...
-00003650: a100 7d0b 7c00 a00c 7c0b a010 a100 640b  ..}.|...|.....d.
-00003660: a102 0100 713c 712c 7124 6400 5300 290c  ....q<q,q$d.S.).
-00003670: 4e72 6600 0000 7287 0000 0072 7e00 0000  Nrf...r....r~...
-00003680: 7288 0000 0072 8900 0000 7285 0000 0072  r....r....r....r
-00003690: 5200 0000 725f 0000 0072 3100 0000 2902  R...r_...r1...).
-000036a0: 727e 0000 0072 8900 0000 7233 0000 0029  r~...r....r3...)
-000036b0: 1172 8b00 0000 7208 0000 0072 0b00 0000  .r....r....r....
-000036c0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-000036d0: 1100 0000 721d 0000 0072 0600 0000 728a  ....r....r....r.
-000036e0: 0000 005a 1867 6574 5f67 726f 7570 6564  ...Z.get_grouped
-000036f0: 5f6d 6170 5f63 6f6e 7465 6e74 7372 0900  _map_contentsr..
-00003700: 0000 721e 0000 0072 1500 0000 726e 0000  ..r....r....rn..
-00003710: 0072 6f00 0000 725f 0000 0029 0c72 2700  .ro...r_...).r'.
-00003720: 0000 722c 0000 0072 2b00 0000 7228 0000  ..r,...r+...r(..
-00003730: 0072 2900 0000 7236 0000 0072 1f00 0000  .r)...r6...r....
-00003740: 722d 0000 00da 0867 726f 7570 5f62 7972  r-.....group_byr
-00003750: 8d00 0000 728e 0000 0072 8f00 0000 722e  ....r....r....r.
-00003760: 0000 0072 2e00 0000 722f 0000 00da 1d74  ...r....r/.....t
-00003770: 6573 745f 6765 745f 6772 6f75 7065 645f  est_get_grouped_
-00003780: 6d61 705f 636f 6e74 656e 7473 c002 0000  map_contents....
-00003790: 732c 0000 0000 0204 0104 020c 010c 0208  s,..............
-000037a0: 0108 0210 0210 020c 0204 0212 0208 0402  ................
-000037b0: 0002 ff02 0402 0002 ff02 fc06 090c 020a  ................
-000037c0: 017a 3b54 6573 744d 6170 436c 7573 7465  .z;TestMapCluste
-000037d0: 7265 7243 6f6e 7465 6e74 436f 756e 7473  rerContentCounts
-000037e0: 2e74 6573 745f 6765 745f 6772 6f75 7065  .test_get_groupe
-000037f0: 645f 6d61 705f 636f 6e74 656e 7473 4e29  d_map_contentsN)
-00003800: 0872 7a00 0000 727b 0000 0072 7c00 0000  .rz...r{...r|...
-00003810: 7290 0000 0072 9400 0000 7297 0000 0072  r....r....r....r
-00003820: 9900 0000 729b 0000 0072 2e00 0000 722e  ....r....r....r.
-00003830: 0000 0072 2e00 0000 722f 0000 0072 7d00  ...r....r/...r}.
-00003840: 0000 e101 0000 730a 0000 0008 0108 6208  ......s.......b.
-00003850: 4408 1d08 1b72 7d00 0000 2922 da0b 646a  D....r}...)"..dj
-00003860: 616e 676f 2e74 6573 7472 0200 0000 da17  ango.testr......
-00003870: 646a 616e 676f 2e63 6f6e 7472 6962 2e67  django.contrib.g
-00003880: 6973 2e67 656f 7372 0300 0000 da17 646a  is.geosr......dj
-00003890: 616e 676f 2e63 6f6e 7472 6962 2e67 6973  ango.contrib.gis
-000038a0: 2e67 6461 6c72 0400 0000 7205 0000 005a  .gdalr....r....Z
-000038b0: 1761 6e79 636c 7573 7465 722e 4d61 7043  .anycluster.MapC
-000038c0: 6c75 7374 6572 6572 7206 0000 00da 0a61  lustererr......a
-000038d0: 6e79 636c 7573 7465 7272 0700 0000 da16  nyclusterr......
-000038e0: 616e 7963 6c75 7374 6572 2e64 6566 696e  anycluster.defin
-000038f0: 6974 696f 6e73 7208 0000 0072 0900 0000  itionsr....r....
-00003900: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00003910: 0d00 0000 5a17 616e 7963 6c75 7374 6572  ....Z.anycluster
-00003920: 2e74 6573 7473 2e63 6f6d 6d6f 6e72 0e00  .tests.commonr..
-00003930: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00003940: 005a 1761 6e79 636c 7573 7465 722e 7465  .Z.anycluster.te
-00003950: 7374 732e 6d69 7869 6e73 7212 0000 0072  sts.mixinsr....r
-00003960: 1300 0000 7214 0000 005a 0d61 6e79 6d61  ....r....Z.anyma
-00003970: 702e 6d6f 6465 6c73 7215 0000 0072 4400  p.modelsr....rD.
-00003980: 0000 721c 0000 0072 8a00 0000 7218 0000  ..r....r....r...
-00003990: 0072 7d00 0000 722e 0000 0072 2e00 0000  .r}...r....r....
-000039a0: 722e 0000 0072 2f00 0000 da08 3c6d 6f64  r....r/.....<mod
-000039b0: 756c 653e 0100 0000 7320 0000 000c 020c  ule>....s ......
-000039c0: 0110 010c 010c 0220 0218 0114 020c 0208  ....... ........
-000039d0: 0204 0104 0214 7f00 7f00 7f00 50         ............P
+00003590: 6772 6964 a502 0000 731a 0000 0000 0204  grid....s.......
+000035a0: 0104 0208 0108 0210 020c 030a 020c 0210  ................
+000035b0: 010e 020a 0204 027a 3854 6573 744d 6170  .......z8TestMap
+000035c0: 436c 7573 7465 7265 7243 6f6e 7465 6e74  ClustererContent
+000035d0: 436f 756e 7473 2e74 6573 745f 736e 6170  Counts.test_snap
+000035e0: 5f76 6965 7770 6f72 745f 746f 5f67 7269  _viewport_to_gri
+000035f0: 6463 0100 0000 0000 0000 0000 0000 0c00  dc..............
+00003600: 0000 0a00 0000 4300 0000 73bc 0000 0064  ......C...s....d
+00003610: 017d 0167 007d 027c 00a0 0064 0264 03a1  .}.g.}.|...d.d..
+00003620: 0201 007c 00a0 0064 0464 05a1 0201 0074  ...|...d.d.....t
+00003630: 0144 005d 927d 0374 0244 005d 887d 0474  .D.].}.t.D.].}.t
+00003640: 0374 0474 0574 0666 0444 005d 767d 057c  .t.t.t.f.D.]v}.|
+00003650: 00a0 077c 047c 017c 037c 02a1 047d 0674  ...|.|.|.|...}.t
+00003660: 087c 0674 0964 068d 027d 0764 077d 087c  .|.t.d...}.d.}.|
+00003670: 07a0 0a7c 057c 047c 017c 027c 08a1 057d  ...|.|.|.|.|...}
+00003680: 097c 0474 0b6b 0272 9864 0864 0969 0164  .|.t.k.r.d.d.i.d
+00003690: 0864 0969 0164 0a9c 027d 0a7c 00a0 0c7c  .d.i.d...}.|...|
+000036a0: 097c 0aa1 0201 0074 0d6a 0ea0 0fa1 007d  .|.....t.j.....}
+000036b0: 0b7c 00a0 0c7c 0ba0 10a1 0064 0ba1 0201  .|...|.....d....
+000036c0: 0071 3c71 2c71 2464 0053 0029 0c4e 726a  .q<q,q$d.S.).Nrj
+000036d0: 0000 0072 8b00 0000 7282 0000 0072 8c00  ...r....r....r..
+000036e0: 0000 728d 0000 0072 8900 0000 7255 0000  ..r....r....rU..
+000036f0: 0072 6200 0000 7234 0000 0029 0272 8200  .rb...r4...).r..
+00003700: 0000 728d 0000 0072 3600 0000 2911 728f  ..r....r6...).r.
+00003710: 0000 0072 0b00 0000 720e 0000 0072 1100  ...r....r....r..
+00003720: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00003730: 0072 2000 0000 7209 0000 0072 8e00 0000  .r ...r....r....
+00003740: da18 6765 745f 6772 6f75 7065 645f 6d61  ..get_grouped_ma
+00003750: 705f 636f 6e74 656e 7473 720c 0000 0072  p_contentsr....r
+00003760: 2100 0000 7218 0000 0072 7200 0000 7273  !...r....rr...rs
+00003770: 0000 0072 6200 0000 290c 722a 0000 0072  ...rb...).r*...r
+00003780: 2f00 0000 722e 0000 0072 2b00 0000 722c  /...r....r+...r,
+00003790: 0000 0072 3900 0000 7222 0000 0072 3000  ...r9...r"...r0.
+000037a0: 0000 da08 6772 6f75 705f 6279 7291 0000  ....group_byr...
+000037b0: 0072 9200 0000 7293 0000 0072 3100 0000  .r....r....r1...
+000037c0: 7231 0000 0072 3200 0000 da1d 7465 7374  r1...r2.....test
+000037d0: 5f67 6574 5f67 726f 7570 6564 5f6d 6170  _get_grouped_map
+000037e0: 5f63 6f6e 7465 6e74 73bf 0200 0073 2c00  _contents....s,.
+000037f0: 0000 0002 0401 0402 0c01 0c02 0801 0802  ................
+00003800: 1002 1002 0c02 0402 1202 0804 0200 02ff  ................
+00003810: 0204 0200 02ff 02fc 0609 0c02 0a01 7a3b  ..............z;
+00003820: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
+00003830: 436f 6e74 656e 7443 6f75 6e74 732e 7465  ContentCounts.te
+00003840: 7374 5f67 6574 5f67 726f 7570 6564 5f6d  st_get_grouped_m
+00003850: 6170 5f63 6f6e 7465 6e74 734e 2908 727e  ap_contentsN).r~
+00003860: 0000 0072 7f00 0000 7280 0000 0072 9400  ...r....r....r..
+00003870: 0000 7298 0000 0072 9b00 0000 729d 0000  ..r....r....r...
+00003880: 0072 a000 0000 7231 0000 0072 3100 0000  .r....r1...r1...
+00003890: 7231 0000 0072 3200 0000 7281 0000 00e1  r1...r2...r.....
+000038a0: 0100 0073 0a00 0000 0801 0862 0844 081d  ...s.......b.D..
+000038b0: 081a 7281 0000 0072 5600 0000 7258 0000  ..r....rV...rX..
+000038c0: 0029 01da 2641 4e59 434c 5553 5445 525f  .)..&ANYCLUSTER_
+000038d0: 4144 4449 5449 4f4e 414c 5f47 524f 5550  ADDITIONAL_GROUP
+000038e0: 5f42 595f 434f 4c55 4d4e 5363 0000 0000  _BY_COLUMNSc....
+000038f0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00003900: 4000 0000 731c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00003910: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00003920: 0464 0553 0029 06da 2354 6573 744d 6170  .d.S.)..#TestMap
+00003930: 436c 7573 7465 7265 7241 6c74 6572 6e61  ClustererAlterna
+00003940: 7469 7665 5365 7474 696e 6773 6301 0000  tiveSettingsc...
+00003950: 0000 0000 0000 0000 000a 0000 0009 0000  ................
+00003960: 0043 0000 0073 6600 0000 6401 7d01 6700  .C...sf...d.}.g.
+00003970: 7d02 7400 4400 5d54 7d03 7401 4400 5d4a  }.t.D.]T}.t.D.]J
+00003980: 7d04 7402 7403 7404 7405 6604 4400 5d38  }.t.t.t.t.f.D.]8
+00003990: 7d05 7c00 a006 7c04 7c01 7c03 7c02 a104  }.|...|.|.|.|...
+000039a0: 7d06 7407 7c06 7408 6402 8d02 7d07 7c07  }.t.|.t.d...}.|.
+000039b0: a009 a100 7d08 6403 7d09 7c00 a00a 7c08  ....}.d.}.|...|.
+000039c0: 7c09 a102 0100 7124 7114 710c 6400 5300  |.....q$q.q.d.S.
+000039d0: 2904 4e72 6a00 0000 7289 0000 007a 3a2c  ).Nrj...r....z:,
+000039e0: 204d 494e 2872 6174 696e 6729 2041 5320   MIN(rating) AS 
+000039f0: 7261 7469 6e67 2c20 4d49 4e28 6c61 7374  rating, MIN(last
+00003a00: 5f72 656e 6577 616c 2920 4153 206c 6173  _renewal) AS las
+00003a10: 745f 7265 6e65 7761 6c29 0b72 0b00 0000  t_renewal).r....
+00003a20: 720e 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00003a30: 1300 0000 7214 0000 0072 2000 0000 7209  ....r....r ...r.
+00003a40: 0000 0072 8e00 0000 5a26 6765 745f 6164  ...r....Z&get_ad
+00003a50: 6469 7469 6f6e 616c 5f67 726f 7570 5f62  ditional_group_b
+00003a60: 795f 636f 6c75 6d6e 735f 7374 7269 6e67  y_columns_string
+00003a70: 7221 0000 0029 0a72 2a00 0000 722f 0000  r!...).r*...r/..
+00003a80: 0072 2e00 0000 722b 0000 0072 2c00 0000  .r....r+...r,...
+00003a90: 7239 0000 0072 2200 0000 7230 0000 005a  r9...r"...r0...Z
+00003aa0: 0e63 6f6c 756d 6e73 5f73 7472 696e 6772  .columns_stringr
+00003ab0: 6800 0000 7231 0000 0072 3100 0000 7232  h...r1...r1...r2
+00003ac0: 0000 00da 2b74 6573 745f 6765 745f 6164  ....+test_get_ad
+00003ad0: 6469 7469 6f6e 616c 5f67 726f 7570 5f62  ditional_group_b
+00003ae0: 795f 636f 6c75 6d6e 735f 7374 7269 6e67  y_columns_string
+00003af0: e902 0000 7314 0000 0000 0204 0104 0208  ....s...........
+00003b00: 0108 0210 0210 020c 0208 0204 017a 4f54  .............zOT
+00003b10: 6573 744d 6170 436c 7573 7465 7265 7241  estMapClustererA
+00003b20: 6c74 6572 6e61 7469 7665 5365 7474 696e  lternativeSettin
+00003b30: 6773 2e74 6573 745f 6765 745f 6164 6469  gs.test_get_addi
+00003b40: 7469 6f6e 616c 5f67 726f 7570 5f62 795f  tional_group_by_
+00003b50: 636f 6c75 6d6e 735f 7374 7269 6e67 6301  columns_stringc.
+00003b60: 0000 0000 0000 0000 0000 000c 0000 000a  ................
+00003b70: 0000 0043 0000 0073 be00 0000 6401 7d01  ...C...s....d.}.
+00003b80: 6700 7d02 7c00 a000 6402 6403 a102 0100  g.}.|...d.d.....
+00003b90: 7c00 a000 6404 6405 a102 0100 7c00 a001  |...d.d.....|...
+00003ba0: 7402 7403 6406 8302 a101 0100 7404 4400  t.t.d.......t.D.
+00003bb0: 5d84 7d03 7405 4400 5d7a 7d04 7406 7407  ].}.t.D.]z}.t.t.
+00003bc0: 7408 7409 6604 4400 5d68 7d05 7c00 a00a  t.t.f.D.]h}.|...
+00003bd0: 7c04 7c01 7c03 7c02 a104 7d06 740b 7c06  |.|.|.|...}.t.|.
+00003be0: 740c 6407 8d02 7d07 6408 7d08 7c07 a00d  t.d...}.d.}.|...
+00003bf0: 7c05 7c04 7c01 7c02 7c08 a105 7d09 7c04  |.|.|.|.|...}.|.
+00003c00: 740e 6b02 724c 7c09 a00f a100 4400 5d20  t.k.rL|.....D.] 
+00003c10: 5c02 7d0a 7d0b 7c00 a010 6409 7c0b a102  \.}.}.|...d.|...
+00003c20: 0100 7c00 a010 640a 7c0b a102 0100 7192  ..|...d.|.....q.
+00003c30: 714c 713c 7134 6400 5300 290b 4e72 6a00  qLq<q4d.S.).Nrj.
+00003c40: 0000 728b 0000 0072 8200 0000 728c 0000  ..r....r....r...
+00003c50: 0072 8d00 0000 72a1 0000 0072 8900 0000  .r....r....r....
+00003c60: 7255 0000 0072 5600 0000 7258 0000 0029  rU...rV...rX...)
+00003c70: 1172 8f00 0000 7227 0000 00da 0768 6173  .r....r'.....has
+00003c80: 6174 7472 7205 0000 0072 0b00 0000 720e  attrr....r....r.
+00003c90: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+00003ca0: 0000 7214 0000 0072 2000 0000 7209 0000  ..r....r ...r...
+00003cb0: 0072 8e00 0000 729e 0000 0072 0c00 0000  .r....r....r....
+00003cc0: da05 6974 656d 73da 0861 7373 6572 7449  ..items..assertI
+00003cd0: 6e29 0c72 2a00 0000 722f 0000 0072 2e00  n).r*...r/...r..
+00003ce0: 0000 722b 0000 0072 2c00 0000 7239 0000  ..r+...r,...r9..
+00003cf0: 0072 2200 0000 7230 0000 0072 9f00 0000  .r"...r0...r....
+00003d00: 7291 0000 00da 0961 6767 7265 6761 7465  r......aggregate
+00003d10: da04 6461 7461 7231 0000 0072 3100 0000  ..datar1...r1...
+00003d20: 7232 0000 00da 3074 6573 745f 6765 745f  r2....0test_get_
+00003d30: 6772 6f75 7065 645f 6d61 705f 636f 6e74  grouped_map_cont
+00003d40: 656e 7473 5f61 6464 6974 696f 6e61 6c5f  ents_additional_
+00003d50: 636f 6c75 6d6e 73fd 0200 0073 2000 0000  columns....s ...
+00003d60: 0002 0401 0402 0c01 0c02 1002 0801 0802  ................
+00003d70: 1002 1002 0c02 0402 1202 0802 1002 0c01  ................
+00003d80: 7a54 5465 7374 4d61 7043 6c75 7374 6572  zTTestMapCluster
+00003d90: 6572 416c 7465 726e 6174 6976 6553 6574  erAlternativeSet
+00003da0: 7469 6e67 732e 7465 7374 5f67 6574 5f67  tings.test_get_g
+00003db0: 726f 7570 6564 5f6d 6170 5f63 6f6e 7465  rouped_map_conte
+00003dc0: 6e74 735f 6164 6469 7469 6f6e 616c 5f63  nts_additional_c
+00003dd0: 6f6c 756d 6e73 4e29 0572 7e00 0000 727f  olumnsN).r~...r.
+00003de0: 0000 0072 8000 0000 72a3 0000 0072 a900  ...r....r....r..
+00003df0: 0000 7231 0000 0072 3100 0000 7231 0000  ..r1...r1...r1..
+00003e00: 0072 3200 0000 72a2 0000 00e5 0200 0073  .r2...r........s
+00003e10: 0400 0000 0804 0814 72a2 0000 0029 27da  ........r....)'.
+00003e20: 0b64 6a61 6e67 6f2e 7465 7374 7202 0000  .django.testr...
+00003e30: 0072 0300 0000 7204 0000 00da 0b64 6a61  .r....r......dja
+00003e40: 6e67 6f2e 636f 6e66 7205 0000 00da 1764  ngo.confr......d
+00003e50: 6a61 6e67 6f2e 636f 6e74 7269 622e 6769  jango.contrib.gi
+00003e60: 732e 6765 6f73 7206 0000 00da 1764 6a61  s.geosr......dja
+00003e70: 6e67 6f2e 636f 6e74 7269 622e 6769 732e  ngo.contrib.gis.
+00003e80: 6764 616c 7207 0000 0072 0800 0000 5a17  gdalr....r....Z.
+00003e90: 616e 7963 6c75 7374 6572 2e4d 6170 436c  anycluster.MapCl
+00003ea0: 7573 7465 7265 7272 0900 0000 da0a 616e  ustererr......an
+00003eb0: 7963 6c75 7374 6572 720a 0000 00da 1661  yclusterr......a
+00003ec0: 6e79 636c 7573 7465 722e 6465 6669 6e69  nycluster.defini
+00003ed0: 7469 6f6e 7372 0b00 0000 720c 0000 0072  tionsr....r....r
+00003ee0: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
+00003ef0: 0000 005a 1761 6e79 636c 7573 7465 722e  ...Z.anycluster.
+00003f00: 7465 7374 732e 636f 6d6d 6f6e 7211 0000  tests.commonr...
+00003f10: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00003f20: 5a17 616e 7963 6c75 7374 6572 2e74 6573  Z.anycluster.tes
+00003f30: 7473 2e6d 6978 696e 7372 1500 0000 7216  ts.mixinsr....r.
+00003f40: 0000 0072 1700 0000 5a0d 616e 796d 6170  ...r....Z.anymap
+00003f50: 2e6d 6f64 656c 7372 1800 0000 7247 0000  .modelsr....rG..
+00003f60: 0072 1f00 0000 728e 0000 0072 1b00 0000  .r....r....r....
+00003f70: 7281 0000 0072 a200 0000 7231 0000 0072  r....r....r1...r
+00003f80: 3100 0000 7231 0000 0072 3200 0000 da08  1...r1...r2.....
+00003f90: 3c6d 6f64 756c 653e 0100 0000 732a 0000  <module>....s*..
+00003fa0: 0014 010c 010c 0110 010c 010c 0220 0218  ............. ..
+00003fb0: 0114 020c 0208 0204 0104 0214 7f00 7f00  ................
+00003fc0: 7f00 5014 7f00 7f00 060c 01              ..P........
```

### Comparing `anycluster-2.3.1/anycluster/tests/common.py` & `anycluster-2.3.2/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/mixins.py` & `anycluster-2.3.2/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/test_ClusterCache.py` & `anycluster-2.3.2/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/test_FilterComposer.py` & `anycluster-2.3.2/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/anycluster/tests/test_MapClusterer.py` & `anycluster-2.3.2/anycluster/tests/test_MapClusterer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from django.test import TestCase
-
+from django.test import TestCase, override_settings, modify_settings
+from django.conf import settings
 from django.contrib.gis.geos import GEOSGeometry
 from django.contrib.gis.gdal import SpatialReference, CoordTransform
 from anycluster.MapClusterer import MapClusterer
 from anycluster import MapTools
 
 from anycluster.definitions import (CLUSTER_TYPES, GEOMETRY_TYPE_VIEWPORT, GEOMETRY_TYPE_AREA, GEOMETRY_TYPES,
                                     CLUSTER_TYPE_KMEANS, CLUSTER_TYPE_GRID)
@@ -451,15 +451,15 @@
 
         filter_lists = self.get_test_filters()
         for filters in filter_lists:
 
             cluster_cache = self.get_cluster_cache(GEOMETRY_TYPE_VIEWPORT, TEST_ZOOM_LEVEL, CLUSTER_TYPE_GRID, filters)
             map_clusterer = MapClusterer(cluster_cache)
 
-            garden_ = map_clusterer.get_dataset_content(garden.id)[0]
+            garden_ = map_clusterer.get_dataset_content(garden.id)
 
             for field_name in map_clusterer.get_gis_field_names():
 
                 if field_name == 'coordinates::bytea':
                     field_name = 'coordinates'
 
                 self.assertEqual(getattr(garden, field_name), getattr(garden_, field_name))
@@ -696,15 +696,14 @@
 
                 grid_rectangle.transform(4326)
 
                 polygon_4326 = 'SRID=4326;POLYGON ((8.7890624999977 47.04018214327889, 14.06249999999632 47.04018214327889, 14.06249999999632 50.7364551355909, 8.7890624999977 50.7364551355909, 8.7890624999977 47.04018214327889))'
 
                 self.assertEqual(polygon_4326, str(grid_rectangle))
 
-
     def test_get_grouped_map_contents(self):
 
         zoom = 10
         filters = []
 
         self.create_point('name 1', 'stone')
         self.create_point('name 2', 'flower')
@@ -732,8 +731,63 @@
                                 'count': 1
                             }
                         }
 
                         self.assertEqual(result, expected_result)
 
                     gardens = Gardens.objects.all()
-                    self.assertEqual(gardens.count(), 2)
+                    self.assertEqual(gardens.count(), 2)
+
+
+@override_settings(ANYCLUSTER_ADDITIONAL_GROUP_BY_COLUMNS = ['rating', 'last_renewal'])
+class TestMapClustererAlternativeSettings(WithFilters, WithGIS, TestCase):
+
+
+    def test_get_additional_group_by_columns_string(self):
+
+        zoom = 10
+        filters = []
+
+        for clustertype in CLUSTER_TYPES:
+            for geometry_type in GEOMETRY_TYPES:
+
+                for geojson in [GEOJSON_POLYGON, GEOJSON_RECTANGLE, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
+
+                    cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
+
+                    map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
+
+                    columns_string = map_clusterer.get_additional_group_by_columns_string()
+
+                    expected_string = ', MIN(rating) AS rating, MIN(last_renewal) AS last_renewal'
+                    self.assertEqual(columns_string, expected_string)
+
+
+    def test_get_grouped_map_contents_additional_columns(self):
+
+        zoom = 10
+        filters = []
+
+        self.create_point('name 1', 'stone')
+        self.create_point('name 2', 'flower')
+
+        self.assertTrue(hasattr(settings, 'ANYCLUSTER_ADDITIONAL_GROUP_BY_COLUMNS'))
+        
+        for clustertype in CLUSTER_TYPES:
+            for geometry_type in GEOMETRY_TYPES:
+
+                for geojson in [GEOJSON_POLYGON, GEOJSON_RECTANGLE, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
+
+                    cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
+
+                    map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
+
+                    group_by = 'style'
+
+                    result = map_clusterer.get_grouped_map_contents(geojson, geometry_type, zoom, filters, group_by)
+
+                    if geometry_type == GEOMETRY_TYPE_VIEWPORT:
+
+                        for aggregate, data in result.items():
+
+                            self.assertIn('rating', data)
+                            self.assertIn('last_renewal', data)
```

### Comparing `anycluster-2.3.1/anycluster.egg-info/PKG-INFO` & `anycluster-2.3.2/anycluster.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.3.1
+Version: 2.3.2
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.3.1/anycluster.egg-info/SOURCES.txt` & `anycluster-2.3.2/anycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.1/setup.py` & `anycluster-2.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.3.1',
+    version='2.3.2',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```

