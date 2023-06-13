# Comparing `tmp/salesea-1.0.34.tar.gz` & `tmp/salesea-1.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.34.tar", last modified: Mon Jun 12 03:22:19 2023, max compression
+gzip compressed data, was "salesea-1.0.35.tar", last modified: Tue Jun 13 01:33:32 2023, max compression
```

## Comparing `salesea-1.0.34.tar` & `salesea-1.0.35.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 03:22:19.247624 salesea-1.0.34/
--rw-rw-rw-   0        0        0     2588 2023-06-12 03:22:19.247624 salesea-1.0.34/PKG-INFO
--rw-rw-rw-   0        0        0     1613 2023-05-29 03:44:29.000000 salesea-1.0.34/README.md
--rw-rw-rw-   0        0        0      111 2023-06-12 03:22:19.248626 salesea-1.0.34/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-06-12 03:19:56.000000 salesea-1.0.34/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:22:19.227626 salesea-1.0.34/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 03:22:19.240625 salesea-1.0.34/src/salesea/
--rw-rw-rw-   0        0        0     6571 2023-05-29 06:18:27.000000 salesea-1.0.34/src/salesea/__command__.py
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.34/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     5833 2023-05-29 06:15:02.000000 salesea-1.0.34/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     8358 2023-06-12 03:21:32.000000 salesea-1.0.34/src/salesea/app.py
--rw-rw-rw-   0        0        0     3580 2023-05-29 06:01:45.000000 salesea-1.0.34/src/salesea/config.py
--rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.34/src/salesea/log.py
--rw-rw-rw-   0        0        0    23808 2023-05-29 08:31:12.000000 salesea-1.0.34/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.34/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.34/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:22:19.246625 salesea-1.0.34/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2588 2023-06-12 03:22:19.000000 salesea-1.0.34/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-06-12 03:22:19.000000 salesea-1.0.34/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 03:22:19.000000 salesea-1.0.34/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-12 03:22:19.000000 salesea-1.0.34/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 03:22:19.000000 salesea-1.0.34/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 03:22:19.000000 salesea-1.0.34/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 01:33:32.789305 salesea-1.0.35/
+-rw-rw-rw-   0        0        0     2588 2023-06-13 01:33:32.789305 salesea-1.0.35/PKG-INFO
+-rw-rw-rw-   0        0        0     1613 2023-05-29 03:44:29.000000 salesea-1.0.35/README.md
+-rw-rw-rw-   0        0        0      111 2023-06-13 01:33:32.790304 salesea-1.0.35/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-06-13 01:33:26.000000 salesea-1.0.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:33:32.770335 salesea-1.0.35/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 01:33:32.782306 salesea-1.0.35/src/salesea/
+-rw-rw-rw-   0        0        0     6571 2023-05-29 06:18:27.000000 salesea-1.0.35/src/salesea/__command__.py
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.35/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     5833 2023-05-29 06:15:02.000000 salesea-1.0.35/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     8607 2023-06-13 01:32:32.000000 salesea-1.0.35/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3580 2023-05-29 06:01:45.000000 salesea-1.0.35/src/salesea/config.py
+-rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.35/src/salesea/log.py
+-rw-rw-rw-   0        0        0    23808 2023-05-29 08:31:12.000000 salesea-1.0.35/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.35/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.35/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:33:32.788306 salesea-1.0.35/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2588 2023-06-13 01:33:32.000000 salesea-1.0.35/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-06-13 01:33:32.000000 salesea-1.0.35/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 01:33:32.000000 salesea-1.0.35/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-13 01:33:32.000000 salesea-1.0.35/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 01:33:32.000000 salesea-1.0.35/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 01:33:32.000000 salesea-1.0.35/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.34/PKG-INFO` & `salesea-1.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.34
+Version: 1.0.35
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `salesea-1.0.34/README.md` & `salesea-1.0.35/README.md`

 * *Files identical despite different names*

### Comparing `salesea-1.0.34/setup.py` & `salesea-1.0.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #     print(requires.splitlines())
 # ------------------------------------------------------------------------------- #
 
 setup(
     name='salesea',
     author='howard',
     author_email='18071131140telephone@gmail.com',
-    version='1.0.34',
+    version='1.0.35',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='This is an Nginx log collection tool.',
     long_description=readme,
     long_description_content_type='text/markdown',
     keywords=[
         'nginx',
```

### Comparing `salesea-1.0.34/src/salesea/__command__.py` & `salesea-1.0.35/src/salesea/__command__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.34/src/salesea/__main__.py` & `salesea-1.0.35/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.34/src/salesea/app.py` & `salesea-1.0.35/src/salesea/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
             print_solution()
             exit(1)
 
         @scheduler(CHECK_INTERVAL)
         def task():
             count = 0
             with requests.session() as sess:
+                ua_set = set()
                 for server in servers:
                     # logger.debug(f"开始扫描日志文件：{[str(server.logfile) for p in servers]}")
                     nginx_log_iter = parse_nginx_log(server.logfile, log_pattern)
 
                     for datas in take(nginx_log_iter, 100):
                         send_data = []
                         for data in datas:
@@ -146,17 +147,21 @@
                                                                   })
                             count += len(send_data)
                             obj = result.json()
                             if obj.get('code') == 'error':
                                 logger.error(f"响应错误: {obj} - {send_data}")
                             else:
                                 logger.info(f"响应结果: {obj}")
+                            for d in send_data:
+                                ua_set.add((d.get('ip'), d.get('user_agent')))
                         except Exception as e:
                             logger.error(f"请求错误: {e} - {send_data}")
 
+            for ip, ua in ua_set:
+                logger.info(f"IP: {ip} - UA: {ua}")
             logger.__getattribute__('info' if count else 'debug')(f"解析到[{count}]条日志")
 
         task()
 
     try:
         from .config import NGINX_PATH, SERVER_MAP, CHECK_INTERVAL, LOG_FORMAT
```

### Comparing `salesea-1.0.34/src/salesea/config.py` & `salesea-1.0.35/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.34/src/salesea/log.py` & `salesea-1.0.35/src/salesea/log.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.34/src/salesea/nginx.py` & `salesea-1.0.35/src/salesea/nginx.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.34/src/salesea/solution.py` & `salesea-1.0.35/src/salesea/solution.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.34/src/salesea.egg-info/PKG-INFO` & `salesea-1.0.35/src/salesea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.34
+Version: 1.0.35
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

