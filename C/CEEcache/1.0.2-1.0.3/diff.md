# Comparing `tmp/CEEcache-1.0.2.tar.gz` & `tmp/CEEcache-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CEEcache-1.0.2.tar", last modified: Fri May 26 05:40:20 2023, max compression
+gzip compressed data, was "CEEcache-1.0.3.tar", last modified: Tue Jun 13 05:25:33 2023, max compression
```

## Comparing `CEEcache-1.0.2.tar` & `CEEcache-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-26 05:40:20.348843 CEEcache-1.0.2/
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-26 05:40:20.344843 CEEcache-1.0.2/CEEcache/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6610 2023-05-26 05:39:02.000000 CEEcache-1.0.2/CEEcache/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1527 2023-05-26 05:39:34.000000 CEEcache-1.0.2/CEEcache/logger.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-26 05:40:20.348843 CEEcache-1.0.2/CEEcache.egg-info/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      604 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      256 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       43 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        9 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/top_level.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       78 2023-05-22 13:09:12.000000 CEEcache-1.0.2/CHANGELOG.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1070 2023-05-22 13:12:22.000000 CEEcache-1.0.2/LICENCE.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       25 2023-05-22 13:10:04.000000 CEEcache-1.0.2/MANIFEST.in
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      604 2023-05-26 05:40:20.348843 CEEcache-1.0.2/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      115 2023-05-22 13:06:57.000000 CEEcache-1.0.2/README.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       38 2023-05-26 05:40:20.348843 CEEcache-1.0.2/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      626 2023-05-26 05:39:48.000000 CEEcache-1.0.2/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-06-13 05:25:33.441506 CEEcache-1.0.3/
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-06-13 05:25:33.441506 CEEcache-1.0.3/CEEcache/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6802 2023-06-13 05:24:39.000000 CEEcache-1.0.3/CEEcache/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1527 2023-05-26 05:39:34.000000 CEEcache-1.0.3/CEEcache/logger.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-06-13 05:25:33.441506 CEEcache-1.0.3/CEEcache.egg-info/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      604 2023-06-13 05:25:33.000000 CEEcache-1.0.3/CEEcache.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      256 2023-06-13 05:25:33.000000 CEEcache-1.0.3/CEEcache.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2023-06-13 05:25:33.000000 CEEcache-1.0.3/CEEcache.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       43 2023-06-13 05:25:33.000000 CEEcache-1.0.3/CEEcache.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        9 2023-06-13 05:25:33.000000 CEEcache-1.0.3/CEEcache.egg-info/top_level.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       78 2023-05-22 13:09:12.000000 CEEcache-1.0.3/CHANGELOG.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1070 2023-05-22 13:12:22.000000 CEEcache-1.0.3/LICENCE.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       25 2023-05-22 13:10:04.000000 CEEcache-1.0.3/MANIFEST.in
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      604 2023-06-13 05:25:33.441506 CEEcache-1.0.3/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      115 2023-05-22 13:06:57.000000 CEEcache-1.0.3/README.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       38 2023-06-13 05:25:33.441506 CEEcache-1.0.3/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      626 2023-06-13 05:24:56.000000 CEEcache-1.0.3/setup.py
```

### Comparing `CEEcache-1.0.2/CEEcache/__init__.py` & `CEEcache-1.0.3/CEEcache/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,22 @@
         send_slack_alert(err_msg, request_id)
         md5_key = None
 
 def send_slack_alert(err_msg, request_id):
     url = os.environ.get("slack_web_hook", "")
     headers = {"Content-Type": "application/json"}
     payload = {"text": err_msg}
-    response = requests.post(url, headers=headers, data=json.dumps(payload))
-    if response.status_code != 200:
-        err_msg = f"Failed to send Slack message. Error: {response.text}"
+    try:
+        response = requests.post(url, headers=headers, data=json.dumps(payload))
+        if response.status_code != 200:
+            err_msg = f"Failed to send Slack message. Error: {response.text}"
+            print(err_msg)
+            log_emmiter({"request_id": request_id, "message": err_msg}, "ERROR")
+    except:
+        err_msg = f"Failed to send Slack message."
         print(err_msg)
         log_emmiter({"request_id": request_id, "message": err_msg}, "ERROR")
 
 def connect_to_redis(request_id):
     max_attempts = 3
     retry_delay = 3
     host = os.environ.get("cache_redis_host", "")
```

### Comparing `CEEcache-1.0.2/CEEcache/logger.py` & `CEEcache-1.0.3/CEEcache/logger.py`

 * *Files identical despite different names*

### Comparing `CEEcache-1.0.2/CEEcache.egg-info/PKG-INFO` & `CEEcache-1.0.3/CEEcache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CEEcache
-Version: 1.0.2
+Version: 1.0.3
 Summary: Caching the JSON request payload and the value in RedisQ
 Home-page: UNKNOWN
 Author: Netcore Cloud
 Author-email: aditya.singh@netcorecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `CEEcache-1.0.2/LICENCE.txt` & `CEEcache-1.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `CEEcache-1.0.2/PKG-INFO` & `CEEcache-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CEEcache
-Version: 1.0.2
+Version: 1.0.3
 Summary: Caching the JSON request payload and the value in RedisQ
 Home-page: UNKNOWN
 Author: Netcore Cloud
 Author-email: aditya.singh@netcorecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `CEEcache-1.0.2/setup.py` & `CEEcache-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='CEEcache',
-  version='1.0.2',
+  version='1.0.3',
   description='Caching the JSON request payload and the value in RedisQ',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Netcore Cloud',
   author_email='aditya.singh@netcorecloud.com',
   license='MIT', 
   classifiers=classifiers,
```

