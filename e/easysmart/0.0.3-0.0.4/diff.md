# Comparing `tmp/easysmart-0.0.3.tar.gz` & `tmp/easysmart-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easysmart-0.0.3.tar", last modified: Tue Jun 13 14:18:37 2023, max compression
+gzip compressed data, was "easysmart-0.0.4.tar", last modified: Tue Jun 13 14:33:13 2023, max compression
```

## Comparing `easysmart-0.0.3.tar` & `easysmart-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:18:37.137242 easysmart-0.0.3/
--rw-rw-rw-   0        0        0       61 2023-06-13 13:52:16.000000 easysmart-0.0.3/.gitignore
--rw-rw-rw-   0        0        0      429 2023-06-13 14:18:37.137242 easysmart-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-06-13 12:56:25.000000 easysmart-0.0.3/README.md
--rw-rw-rw-   0        0        0        0 2023-06-13 12:43:50.000000 easysmart-0.0.3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:18:37.127123 easysmart-0.0.3/easysmart/
--rw-rw-rw-   0        0        0       69 2023-06-13 14:15:41.000000 easysmart-0.0.3/easysmart/__init__.py
--rw-rw-rw-   0        0        0       36 2023-06-13 12:45:18.000000 easysmart-0.0.3/easysmart/func.py
--rw-rw-rw-   0        0        0     2337 2023-06-13 14:06:47.000000 easysmart-0.0.3/easysmart/manager.py
--rw-rw-rw-   0        0        0     1312 2023-06-13 13:50:31.000000 easysmart-0.0.3/easysmart/mdns.py
--rw-rw-rw-   0        0        0      850 2023-06-13 13:54:37.000000 easysmart-0.0.3/easysmart/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:18:37.135123 easysmart-0.0.3/easysmart.egg-info/
--rw-rw-rw-   0        0        0      429 2023-06-13 14:18:37.000000 easysmart-0.0.3/easysmart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-13 14:18:37.000000 easysmart-0.0.3/easysmart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:18:37.000000 easysmart-0.0.3/easysmart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 14:18:37.000000 easysmart-0.0.3/easysmart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 14:18:37.138255 easysmart-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-06-13 14:18:27.000000 easysmart-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:33:13.202501 easysmart-0.0.4/
+-rw-rw-rw-   0        0        0       61 2023-06-13 13:52:16.000000 easysmart-0.0.4/.gitignore
+-rw-rw-rw-   0        0        0      429 2023-06-13 14:33:13.202501 easysmart-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-06-13 12:56:25.000000 easysmart-0.0.4/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-13 12:43:50.000000 easysmart-0.0.4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:33:13.190502 easysmart-0.0.4/easysmart/
+-rw-rw-rw-   0        0        0       69 2023-06-13 14:28:19.000000 easysmart-0.0.4/easysmart/__init__.py
+-rw-rw-rw-   0        0        0       36 2023-06-13 12:45:18.000000 easysmart-0.0.4/easysmart/func.py
+-rw-rw-rw-   0        0        0     2337 2023-06-13 14:06:47.000000 easysmart-0.0.4/easysmart/manager.py
+-rw-rw-rw-   0        0        0     1312 2023-06-13 13:50:31.000000 easysmart-0.0.4/easysmart/mdns.py
+-rw-rw-rw-   0        0        0      850 2023-06-13 13:54:37.000000 easysmart-0.0.4/easysmart/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:33:13.199500 easysmart-0.0.4/easysmart.egg-info/
+-rw-rw-rw-   0        0        0      429 2023-06-13 14:33:13.000000 easysmart-0.0.4/easysmart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-13 14:33:13.000000 easysmart-0.0.4/easysmart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:33:13.000000 easysmart-0.0.4/easysmart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-13 14:33:13.000000 easysmart-0.0.4/easysmart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 14:33:13.000000 easysmart-0.0.4/easysmart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:33:13.203500 easysmart-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1402 2023-06-13 14:33:10.000000 easysmart-0.0.4/setup.py
```

### Comparing `easysmart-0.0.3/easysmart/manager.py` & `easysmart-0.0.4/easysmart/manager.py`

 * *Files identical despite different names*

### Comparing `easysmart-0.0.3/easysmart/mdns.py` & `easysmart-0.0.4/easysmart/mdns.py`

 * *Files identical despite different names*

### Comparing `easysmart-0.0.3/easysmart/utils.py` & `easysmart-0.0.4/easysmart/utils.py`

 * *Files identical despite different names*

### Comparing `easysmart-0.0.3/setup.py` & `easysmart-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="easysmart",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.0.3",
+    version="0.0.4",
     # 作者名
     author="jiandanzhineng",
     # 作者邮箱
     author_email="jiandanzhineng@outlook.com",
     # 包的简介描述
     description="简单智能官方实现",
     # 包的详细介绍(一般通过加载README.md)
     long_description=long_description,
     # 和上条命令配合使用，声明加载的是markdown文件
     long_description_content_type="text/markdown",
     # 项目开源地址
     url="https://baidu.com",
     # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
     packages=setuptools.find_packages(),
+    install_requires=['paho-mqtt', 'zeroconf', 'requests'],
     # 关于包的其他元数据(metadata)
     classifiers=[
         # 该软件包仅与Python3兼容
         "Programming Language :: Python :: 3",
         # 根据MIT许可证开源
         "License :: OSI Approved :: MIT License",
         # 与操作系统无关
```

