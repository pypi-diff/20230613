# Comparing `tmp/meili_ros_lib-0.1.5.tar.gz` & `tmp/meili_ros_lib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili_ros_lib-0.1.5.tar", last modified: Fri Apr 28 17:18:06 2023, max compression
+gzip compressed data, was "meili_ros_lib-0.1.6.tar", last modified: Tue Jun 13 08:52:48 2023, max compression
```

## Comparing `meili_ros_lib-0.1.5.tar` & `meili_ros_lib-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 nuriafe   (1001) nuriafe   (1001)        0 2023-04-28 17:18:06.746727 meili_ros_lib-0.1.5/
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)     1085 2023-01-24 09:48:58.000000 meili_ros_lib-0.1.5/LICENSE.txt
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)      294 2023-04-28 17:18:06.746727 meili_ros_lib-0.1.5/PKG-INFO
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)       14 2023-04-28 15:15:34.000000 meili_ros_lib-0.1.5/README.md
-drwxrwxr-x   0 nuriafe   (1001) nuriafe   (1001)        0 2023-04-28 17:18:06.746727 meili_ros_lib-0.1.5/meili_ros_lib/
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)        0 2023-03-09 09:53:39.000000 meili_ros_lib-0.1.5/meili_ros_lib/__init__.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)    20850 2023-04-28 15:15:34.000000 meili_ros_lib-0.1.5/meili_ros_lib/agent.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)     2208 2023-03-09 13:07:28.000000 meili_ros_lib-0.1.5/meili_ros_lib/agent_setup.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)     4521 2023-03-09 09:53:39.000000 meili_ros_lib-0.1.5/meili_ros_lib/config_agent.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)     3274 2023-03-14 14:12:13.000000 meili_ros_lib-0.1.5/meili_ros_lib/connection.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)     1450 2023-03-09 09:53:39.000000 meili_ros_lib-0.1.5/meili_ros_lib/docking.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)     1649 2023-03-09 09:53:39.000000 meili_ros_lib-0.1.5/meili_ros_lib/maths.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)    11990 2023-03-09 09:53:39.000000 meili_ros_lib-0.1.5/meili_ros_lib/offline.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)     2620 2023-03-09 14:18:23.000000 meili_ros_lib-0.1.5/meili_ros_lib/parse_data.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)     9864 2023-04-28 15:15:34.000000 meili_ros_lib-0.1.5/meili_ros_lib/sdk_handlers.py
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)      881 2023-03-09 09:53:39.000000 meili_ros_lib-0.1.5/meili_ros_lib/sentry.py
-drwxrwxr-x   0 nuriafe   (1001) nuriafe   (1001)        0 2023-04-28 17:18:06.746727 meili_ros_lib-0.1.5/meili_ros_lib.egg-info/
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)      294 2023-04-28 17:18:06.000000 meili_ros_lib-0.1.5/meili_ros_lib.egg-info/PKG-INFO
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)      479 2023-04-28 17:18:06.000000 meili_ros_lib-0.1.5/meili_ros_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)        1 2023-04-28 17:18:06.000000 meili_ros_lib-0.1.5/meili_ros_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)       14 2023-04-28 17:18:06.000000 meili_ros_lib-0.1.5/meili_ros_lib.egg-info/top_level.txt
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)      345 2023-04-28 17:18:06.746727 meili_ros_lib-0.1.5/setup.cfg
--rw-rw-r--   0 nuriafe   (1001) nuriafe   (1001)      131 2023-01-24 12:34:21.000000 meili_ros_lib-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:52:48.179891 meili_ros_lib-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 08:52:48.179891 meili_ros_lib-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:52:48.178891 meili_ros_lib-0.1.6/meili_ros_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20850 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/agent_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/config_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/docking.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/maths.py
+-rw-rw-rw-   0 root         (0) root         (0)    11990 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/offline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/parse_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     9864 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/sdk_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/meili_ros_lib/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:52:48.179891 meili_ros_lib-0.1.6/meili_ros_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 08:52:48.000000 meili_ros_lib-0.1.6/meili_ros_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-13 08:52:48.000000 meili_ros_lib-0.1.6/meili_ros_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:52:48.000000 meili_ros_lib-0.1.6/meili_ros_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 08:52:48.000000 meili_ros_lib-0.1.6/meili_ros_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-13 08:52:48.180891 meili_ros_lib-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-13 08:52:38.000000 meili_ros_lib-0.1.6/setup.py
```

### Comparing `meili_ros_lib-0.1.5/LICENSE.txt` & `meili_ros_lib-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/agent.py` & `meili_ros_lib-0.1.6/meili_ros_lib/agent.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/agent_setup.py` & `meili_ros_lib-0.1.6/meili_ros_lib/agent_setup.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/config_agent.py` & `meili_ros_lib-0.1.6/meili_ros_lib/config_agent.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/connection.py` & `meili_ros_lib-0.1.6/meili_ros_lib/connection.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/docking.py` & `meili_ros_lib-0.1.6/meili_ros_lib/docking.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/maths.py` & `meili_ros_lib-0.1.6/meili_ros_lib/maths.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/offline.py` & `meili_ros_lib-0.1.6/meili_ros_lib/offline.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/parse_data.py` & `meili_ros_lib-0.1.6/meili_ros_lib/parse_data.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/sdk_handlers.py` & `meili_ros_lib-0.1.6/meili_ros_lib/sdk_handlers.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.5/meili_ros_lib/sentry.py` & `meili_ros_lib-0.1.6/meili_ros_lib/sentry.py`

 * *Files identical despite different names*

