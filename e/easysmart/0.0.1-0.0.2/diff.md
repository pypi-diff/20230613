# Comparing `tmp/easysmart-0.0.1.tar.gz` & `tmp/easysmart-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easysmart-0.0.1.tar", last modified: Tue Jun 13 12:57:00 2023, max compression
+gzip compressed data, was "easysmart-0.0.2.tar", last modified: Tue Jun 13 14:12:34 2023, max compression
```

## Comparing `easysmart-0.0.1.tar` & `easysmart-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:57:00.980223 easysmart-0.0.1/
--rw-rw-rw-   0        0        0      423 2023-06-13 12:57:00.979224 easysmart-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-06-13 12:56:25.000000 easysmart-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 12:57:00.969221 easysmart-0.0.1/easysmart/
--rw-rw-rw-   0        0        0        0 2023-06-13 12:44:32.000000 easysmart-0.0.1/easysmart/__init__.py
--rw-rw-rw-   0        0        0       36 2023-06-13 12:45:18.000000 easysmart-0.0.1/easysmart/func.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:57:00.977223 easysmart-0.0.1/easysmart.egg-info/
--rw-rw-rw-   0        0        0      423 2023-06-13 12:57:00.000000 easysmart-0.0.1/easysmart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-13 12:57:00.000000 easysmart-0.0.1/easysmart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:57:00.000000 easysmart-0.0.1/easysmart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 12:57:00.000000 easysmart-0.0.1/easysmart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 12:57:00.980223 easysmart-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1335 2023-06-13 12:56:54.000000 easysmart-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:12:34.815380 easysmart-0.0.2/
+-rw-rw-rw-   0        0        0       61 2023-06-13 13:52:16.000000 easysmart-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0      429 2023-06-13 14:12:34.813992 easysmart-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-06-13 12:56:25.000000 easysmart-0.0.2/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-13 12:43:50.000000 easysmart-0.0.2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:12:34.804205 easysmart-0.0.2/easysmart/
+-rw-rw-rw-   0        0        0       39 2023-06-13 14:06:39.000000 easysmart-0.0.2/easysmart/__init__.py
+-rw-rw-rw-   0        0        0       36 2023-06-13 12:45:18.000000 easysmart-0.0.2/easysmart/func.py
+-rw-rw-rw-   0        0        0     2337 2023-06-13 14:06:47.000000 easysmart-0.0.2/easysmart/manager.py
+-rw-rw-rw-   0        0        0     1312 2023-06-13 13:50:31.000000 easysmart-0.0.2/easysmart/mdns.py
+-rw-rw-rw-   0        0        0      850 2023-06-13 13:54:37.000000 easysmart-0.0.2/easysmart/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:12:34.811206 easysmart-0.0.2/easysmart.egg-info/
+-rw-rw-rw-   0        0        0      429 2023-06-13 14:12:34.000000 easysmart-0.0.2/easysmart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-13 14:12:34.000000 easysmart-0.0.2/easysmart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:12:34.000000 easysmart-0.0.2/easysmart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 14:12:34.000000 easysmart-0.0.2/easysmart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:12:34.815380 easysmart-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-06-13 14:05:24.000000 easysmart-0.0.2/setup.py
```

### Comparing `easysmart-0.0.1/setup.py` & `easysmart-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="easysmart",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.0.1",
+    version="0.0.2",
     # 作者名
     author="jiandanzhineng",
     # 作者邮箱
     author_email="jiandanzhineng@outlook.com",
     # 包的简介描述
     description="简单智能官方实现",
     # 包的详细介绍(一般通过加载README.md)
@@ -25,10 +25,10 @@
     # 关于包的其他元数据(metadata)
     classifiers=[
         # 该软件包仅与Python3兼容
         "Programming Language :: Python :: 3",
         # 根据MIT许可证开源
         "License :: OSI Approved :: MIT License",
         # 与操作系统无关
-        "Operating System :: OS Independent",
+        "Operating System :: Microsoft :: Windows",
     ],
 )
```

