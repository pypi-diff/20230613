# Comparing `tmp/sotest_utils-0.1.7.tar.gz` & `tmp/sotest_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sotest_utils-0.1.7.tar", last modified: Sun Oct  9 06:52:44 2022, max compression
+gzip compressed data, was "sotest_utils-0.1.8.tar", last modified: Tue Jun 13 02:32:48 2023, max compression
```

## Comparing `sotest_utils-0.1.7.tar` & `sotest_utils-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)        0 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      186 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/PKG-INFO
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      380 2022-08-23 09:57:17.000000 sotest_utils-0.1.7/README.md
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      189 2022-10-09 06:52:37.000000 sotest_utils-0.1.7/setup.py
-drwxr-xr-x   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)        0 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/sotest_utils/
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)     4634 2022-08-23 09:57:17.000000 sotest_utils-0.1.7/sotest_utils/magic.py
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      102 2022-09-13 03:27:23.000000 sotest_utils-0.1.7/sotest_utils/__init__.py
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)     1053 2022-09-30 08:46:02.000000 sotest_utils-0.1.7/sotest_utils/test.py
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)       38 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/setup.cfg
-drwxr-xr-x   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)        0 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/sotest_utils.egg-info/
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      186 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/sotest_utils.egg-info/PKG-INFO
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      265 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/sotest_utils.egg-info/SOURCES.txt
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)       42 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/sotest_utils.egg-info/requires.txt
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)       13 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/sotest_utils.egg-info/top_level.txt
--rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)        1 2022-10-09 06:52:44.000000 sotest_utils-0.1.7/sotest_utils.egg-info/dependency_links.txt
+drwxr-xr-x   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)        0 2023-06-13 02:32:48.865201 sotest_utils-0.1.8/
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)       56 2023-06-13 02:32:48.865027 sotest_utils-0.1.8/PKG-INFO
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      380 2022-08-23 09:57:17.000000 sotest_utils-0.1.8/README.md
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)       38 2023-06-13 02:32:48.865247 sotest_utils-0.1.8/setup.cfg
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      189 2023-06-13 02:30:34.000000 sotest_utils-0.1.8/setup.py
+drwxr-xr-x   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)        0 2023-06-13 02:32:48.860826 sotest_utils-0.1.8/sotest_utils/
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      102 2022-09-13 03:27:23.000000 sotest_utils-0.1.8/sotest_utils/__init__.py
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)     4634 2022-08-23 09:57:17.000000 sotest_utils-0.1.8/sotest_utils/magic.py
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)     1122 2023-06-13 02:29:56.000000 sotest_utils-0.1.8/sotest_utils/test.py
+drwxr-xr-x   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)        0 2023-06-13 02:32:48.864841 sotest_utils-0.1.8/sotest_utils.egg-info/
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)       56 2023-06-13 02:32:48.000000 sotest_utils-0.1.8/sotest_utils.egg-info/PKG-INFO
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)      265 2023-06-13 02:32:48.000000 sotest_utils-0.1.8/sotest_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)        1 2023-06-13 02:32:48.000000 sotest_utils-0.1.8/sotest_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)       42 2023-06-13 02:32:48.000000 sotest_utils-0.1.8/sotest_utils.egg-info/requires.txt
+-rw-r--r--   0 10027865 (314065474) SHEIN-INC\Domain Users (1137481367)       13 2023-06-13 02:32:48.000000 sotest_utils-0.1.8/sotest_utils.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sotest_utils-0.1.7/sotest_utils/magic.py` & `sotest_utils-0.1.8/sotest_utils/magic.py`

 * *Files identical despite different names*

### Comparing `sotest_utils-0.1.7/sotest_utils/test.py` & `sotest_utils-0.1.8/sotest_utils/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 from inspect import isfunction
 
 
-def sotest_test_case(test_name="", group="", author="", level="", cmdb_name="", cid=""):
+def sotest_test_case(test_name="", group="", author="", level="", cmdb_name="", cid="", case_desc=""):
     """
     sotest test case扫描标识
     :param test_name: 用例名称
     :param group: 用例分组，用于soTest页面展示分组
     :param author: 作者，用于标记
     :param level: 用例级别：L1: 冒烟测试用例，L2: 重要功能用例，L3: 一般功能用例，L4: 生僻功能用例
     :param cmdb_name: 系统名称
     :param cid: 用例uuid唯一标识，在项目中需要保证其唯一性，用于用例更新时匹配的id，未配置时使用：package + class + method name,
                 在线生成地址：https://www.guidgenerator.com/
+    :param case_desc 用例描述
     :return:
     """
     name = test_name
     if isfunction(test_name):
         name = test_name.__name__
     import allure
     return allure.label("sotest_test_case",
                         json.dumps(dict(test_name=name, group=group, author=author, level=level, cmdb_name=cmdb_name,
-                                        cid=cid)))
+                                        cid=cid, case_desc=case_desc)))
```

